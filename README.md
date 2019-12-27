# MSTN_IAR_DAC_SineWave

This example describes how to use DAC with DMA to generate sine waves on DAC channel output.
Configure PORTE line 0 as DAC2_OUT .
DMA channel10 is configured to transfer ping-pong mode, word by word, a 32-word buffer to DAC register DAC2_DATA.
The transfered 32 buffer is made to have a sine wave generation on DAC channel output. DAC channel2 is enabled.
Once TIM1 is enabled, each TIM1 CNT_ARR_EVENT generate a DMA request which transfer data to the  DAC2_DATA register and DAC conversion is started. The sine waves can be visualized by connecting DAC_OUT jack to an oscilloscope.

