Raspberry Pi 4 ADC acquisition

Please run the following code to initiate

`gcc -Wall -o rpi_adc_stream rpi_adc_stream.c rpi_dma_utils.c`

`sudo ./rpi_adc_stream -n 1000 -r 250000 -s /tmp/adc.fifo`

`cat /tmp/adc.fifo > adc_reading.csv`

Thank you Jeremy for your amazing RPI DMA library and your amazing blog on DMA. https://iosoft.blog/2020/05/25/raspberry-pi-dma-programming/
