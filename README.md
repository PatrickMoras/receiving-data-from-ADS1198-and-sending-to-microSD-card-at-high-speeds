# receiving-data-from-ADS1198-and-sending-to-microSD-card-at-high-speeds

_____________________________________________________________________________________________________________________________________________
**author:** Patrick Morás
**Data:** 30/07/2021           
**Objetivo:** Analysis of problems in the transmission of data by DMA to microSD card while receiving data from another device (in this case the ADS1198) with DMA. Receive data at a frequency of 1KHz, process it and save it to microSD card.
**IDE=** STM32CUBE IDE v.1.7.0
**GUI=** TouchGFX v.4.17.0

# problem description
_____________________________________________________________________________________________________________________________________________
Using the same Direct Memory Access (DMA2) as the STM32F7 platform to receive data from the ADS1198 and transmit it to the microSD Card at a frequency of 1ms results in: functions managing DMA crashing or ADS1198 stopping sending data. Evaluating the times of receiving data from the ADS1198 and sending it to the microSD card on the oscilloscope, a delay in recording to the microSD was noted periodically with more than 1ms of time.



_____________________________________________________________________________________________________________________________________________
# More Information

- First steps with [SD card and STM32](https://www.youtube.com/watch?v=I9KDN1o6924)
- Some solutions for [errors between FatFS and STM32](https://pcbartists.com/firmware/stm32-firmware/hard-fault-stm32-fatfs-solutions/)
- SD Card Write Delays Due to [Internal SD Card Operations When Exceeding Sector Memory](https://www.microchip.com/forums/m577927.aspx)
