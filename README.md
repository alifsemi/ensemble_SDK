## AlifSemi Ensemble_SDK Overview
AlifSemi Ensemble SDK provides all the necessary instructions and tools to facilitate development of applications on Ensemble processors.

AlifSemi Ensemble SDK includes:
* Geting started guides and application notes
* Tools for security and product configuration
* Example applications and templates
* Support for multiple tool chains - VSCode, Keil MDK
* Support for multiple compilers - GCC, Arm Clang
* Support for multiple RTOSes - Azure RTOS, FreeRTOS (coming soon), and Zephyr (coming soon)
* Support for Ensemble Evaluation Kits

## Content Description
This repository is intended to provide a summarry of all the Ensemble SDK related GitHub projects.

### General guidelines 
- Most Ensemble SDK examples are designed to run on the M55 (HE/HP) cores in the Real Time Sub-System (RTSS) 
- RTSS example applications are built by default using either HP or HE core. The selected core is a build option and can be changed 
- Camera examples do not run on E1 devices due to different camera interface – only LP-Parallel is supported on E1.     

### Ensemble Embedded Software packages
Ensemble Packages | Description | E7 | E5 | E3 | E1
------------------| ----------- | ---| -- | -- | --| 
[Ensemble CMSIS DFP](https://github.com/alifsemi/alif_ensemble-cmsis-dfp) | Ensemble CMSIS DFP | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE
[Ensemble Azure RTOS pack](https://github.com/alifsemi/alif_ensemble-Azure-RTOS) | Ensemble Azure RTOS support pack | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE  
[Ensemble FreeRTOS pack](https://github.com/alifsemi/alif_ensemble-FreeRTOS-Components) | Ensemble FreeRTOS support pack | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE  
[VS Code template](https://github.com/alifsemi/alif_vscode-template) | Ensemble VS Code template | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE
[Ensemble boardlib](https://github.com/alifsemi/alif_boardlib) | Ensemble boardlib | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE
[Ensemble ML](https://github.com/alifsemi/alif_ml-embedded-evaluation-kit) | Ensemble ML evaluation kit | M55 HE/HP (1) | M55 HE/HP (1) | M55 HE/HP (1) | KWS only  
[Ensemble CMSIS based ML example](https://github.com/alifsemi/alif_mlek-cmsis-examples) | Ensemble CMSIS-Pack based ML Example | M55 HE/HP | M55 HE/HP | M55 HE/HP | KWS only  
[Ensemble Multicore Azure RTOS](https://github.com/alifsemi/alif_ensemble-vscode-multicore) | Ensemble Azure RTOS CMSIS Pack | M55 HE/HP | M55 HE/HP | M55 HE/HP | N.A.  
[Viewfinder example application](https://github.com/alifsemi/alif_M55-viewfinder) | Ensemble Viewfinder example application | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE  
[Common Application Utilities](https://github.com/alifsemi/alif_common-app-utils) | Ensemble Common Application Utilities | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE  
[Conductor Tool Demo Application](https://github.com/alifsemi/alif_conductor-demo) | Demo application for Conductor Tool worflow | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE  
[MP3 Player Demo](https://github.com/alifsemi/alif_mp3player) | MP3 Player with GUI Demo application | M55 HE/HP (2) | M55 HE/HP (2) | M55 HE/HP (2) | M55 HE (2)  
[MCUboot example](https://github.com/alifsemi/alif_mcuboot_example) | MCUboot Example for Alif Ensemble | M55 HE (3) | M55 HE (3) | M55 HE (3) | M55 HE (3)  
[Low Power Demo: Sensor Sampling](https://github.com/alifsemi/alif_LowPower_SensorSampling) | A use-case based low power demo for Alif Ensemble E1 and E3 processors. | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE

(1) Any model can be run on any core and the limiting factor is the model’s memory requirements and the used memory configuration. Alif provides a reference memory configuration (scripts/cmake/platforms/ensemble) but users can modify these to match their needs. With Alif reference memory configuration some typical use cases are run as follows: 
- Alif KWS: M55 HE 
- Alif Image Classification: M55 HP 
- Alif Object Detection: M55 HP 
- Inference runner: M55 HE or M55 HP 

(2) Requires audio output for sound. On Alif boards, only AppKit has audio output. Application runs on DevKit also, but without sound output. 

(3) Currently linker configuration is provided to M55 HE only but should be easy to port to work on M55 HP also. 

## Tools
* Alif Security Tool (Available on Evaluation Kit specific web page linked below)
* [Alif Conductor](https://conductor.alifsemi.com/)

## Documentation
* Data Sheets (Available on Evaluation Kit specific web page linked below)
* Reference Manuals (Available on Evaluation Kit specific web page linked below)
* Schematics (Available on Evaluation Kit specific web page linked below)

## Compatible evaluation kits
* [Gen 2 Ensemble Development kit](https://alifsemi.com/support/kits/ensemble-devkit-gen2/)
* [Gen 1 Ensemble ML/AI Application kit](https://alifsemi.com/support/kits/ai-ml-appkit/)

## FAQ
To view the FAQs, please visit
* [Alif FAQs](https://alifsemi.com/support/faqs/)
## Support
For support, please visit
* [Alif Support](https://alifsemi.com/support/technical-support/) to submit your support tickets
