## Alif Semiconductor Software Development Kit (SDK) Overview
Alif Semiconductor SDK provides all the necessary instructions and tools to facilitate development of applications on Ensemble and Balleto processors.

Alif Semiconductor SDK includes:
* Geting started guides and application notes
* Tools for security and product configuration
* Example applications and templates
* Support for multiple tool chains - VSCode, Keil MDK
* Support for multiple compilers - GCC, Arm Clang
* Support for multiple RTOSes - Azure RTOS, FreeRTOS, and Zephyr
* Support for Ensemble Evaluation Kits

## Content Description
This repository is intended to provide a summarry of all the SDK related GitHub projects.

### General guidelines
- Most Ensemble SDK examples are designed to run on the M55 (HE/HP) cores in the Real Time Sub-System (RTSS)
- RTSS example applications are built by default using either HP or HE core. The selected core is a build option and can be changed
- Camera examples do not run on E1/E1C/B1 devices due to different camera interface – only LP-Parallel is supported on E1/E1C/B1.

### Embedded Software packages
Packages | Description | E7 | E5 | E3 | E1/E1C | B1
------------------| ----------- | ---| -- | -- | --| --|
[VS Code template](https://github.com/alifsemi/alif_vscode-template) | Ensemble VS Code template. **START HERE** | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[Ensemble CMSIS DFP](https://github.com/alifsemi/alif_ensemble-cmsis-dfp) | Ensemble CMSIS DFP | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE
[Ensemble Azure RTOS pack](https://github.com/alifsemi/alif_ensemble-Azure-RTOS) | Ensemble Azure RTOS support pack | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[Ensemble Azure examples](https://github.com/alifsemi/alif_ensemble-vscode-azure-examples) | Ensemble Azure examples | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[Ensemble Multicore Azure RTOS example](https://github.com/alifsemi/alif_ensemble-vscode-multicore) | Ensemble Azure RTOS CMSIS Pack | M55 HE/HP | M55 HE/HP | M55 HE/HP | N.A. | N.A.
[Ensemble FreeRTOS pack](https://github.com/alifsemi/alif_ensemble-FreeRTOS-Components) | Ensemble FreeRTOS support pack | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[FreeRTOS blinky example](https://github.com/alifsemi/alif_vscode-freertos-blinky) | Simple Blinky example with FreeRTOS | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[Ensemble boardlib](https://github.com/alifsemi/alif_boardlib) | Ensemble boardlib | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[Common Application Utilities](https://github.com/alifsemi/alif_common-app-utils) | Ensemble Common Application Utilities | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[Ensemble ML](https://github.com/alifsemi/alif_ml-embedded-evaluation-kit) | Ensemble ML evaluation kit | M55 HE/HP (1) | M55 HE/HP (1) | M55 HE/HP (1) | KWS only | KWS only
[Ensemble CMSIS based ML example](https://github.com/alifsemi/alif_mlek-cmsis-examples) | Ensemble CMSIS-Pack based ML Example | M55 HE/HP | M55 HE/HP | M55 HE/HP | KWS only | KWS only
[Viewfinder example application](https://github.com/alifsemi/alif_M55-viewfinder) | Ensemble Viewfinder example application | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[Conductor Tool Demo Application](https://github.com/alifsemi/alif_conductor-demo) | Demo application for Conductor Tool worflow | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[MP3 Player Demo](https://github.com/alifsemi/alif_mp3player) | MP3 Player with GUI Demo application | M55 HE/HP (2) | M55 HE/HP (2) | M55 HE/HP (2) | M55 HE (2) | M55 HE (4)
[MCUboot example](https://github.com/alifsemi/alif_mcuboot_example) | MCUboot Example for Alif Ensemble | M55 HE (3) | M55 HE (3) | M55 HE (3) | M55 HE | M55 HE (4)
[aiPM VSCode Example](https://github.com/alifsemi/alif_ensemble-vscode-aiPMExamples) | VSCode project for CMSIS Pack aiPM Examples | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[Low Power Demo: Sensor Sampling](https://github.com/alifsemi/alif_LowPower_SensorSampling) | A use-case based low power demo for Alif Ensemble E1 and E3 processors | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[OSPI flasher example](https://github.com/alifsemi/alif_sd-to-ospi-flasher) | Programming OSPI flash from SD card demo | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[TinyUSB baremetal example](https://github.com/alifsemi/alif_m55-lvgl) | M55 LVGL Demo | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE (4)
[Zephyr SDK](https://github.com/alifsemi/sdk-alif) | Starting point for Zephyr development on Alif devices | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE
[Zephyr HAL for Alif](https://github.com/alifsemi/hal_alif) | Zephyr HAL port for Alif | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE
[Zephyr OS for Alif](https://github.com/alifsemi/zephyr_alif) | Zephyr Project OS port for Alif | M55 HE/HP | M55 HE/HP | M55 HE/HP | M55 HE | M55 HE

(1) Any model can be run on any core and the limiting factor is the model’s memory requirements and the used memory configuration. Alif provides a reference memory configuration (scripts/cmake/platforms/ensemble) but users can modify these to match their needs. With Alif reference memory configuration some typical use cases are run as follows:
- Alif KWS: M55 HE
- Alif Image Classification: M55 HP
- Alif Object Detection: M55 HP
- Inference runner: M55 HE or M55 HP

(2) Requires audio output for sound. On Alif boards, only AppKit has audio output. Application runs on DevKit also, but without sound output.

(3) Currently linker configuration is provided to M55 HE only but should be easy to port to work on M55 HP also.

(4) Use the E1C project for M55-HE on B1.

## Tools
* Alif Security Tool (Wondows, Linux, and MacOS versions available at [Software & Tools](https://alifsemi.com/support/software-tools/ensemble/))
* [Alif Conductor](https://conductor.alifsemi.com/)

## Documentation
* Schematics (Available on Evaluation Kit specific web page linked below)
* [Datasheets](https://alifsemi.com/support/datasheets/ensemble/)
* [Reference Manuals](https://alifsemi.com/support/reference-manuals/ensemble/)
* [User Guide & App Notes](https://alifsemi.com/support/application-notes-user-guides/ensemble/)
* [Whitepapers](https://alifsemi.com/whitepapers/)
* [Case Studies](https://alifsemi.com/case-studies/)
### Some Early Versions of Docmentation Released on GItHub
* [How to Import Project to VSCode](./earlydocs/NewProcjectImportToVSCode.md)

## Compatible evaluation kits
* [Gen 2 Ensemble Development kit](https://alifsemi.com/support/kits/ensemble-devkit-gen2/)
* [Gen 2 Ensemble ML/AI Application kit](https://alifsemi.com/support/kits/ai-ml-appkit-gen-2/)

## Additional Resources
* [Webinars](https://alifsemi.com/webinars/)
* [Partners](https://alifsemi.com/partners/)

## FAQ
To view the FAQs, please visit
* [Alif FAQs](https://alifsemi.com/support/faqs/)

## Support
For support, please visit
* [Alif Support](https://alifsemi.com/support/technical-support/) to submit your support tickets
