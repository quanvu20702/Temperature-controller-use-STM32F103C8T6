# Temperature-controller-use-STM32F103C8T6
STM32F103C8T6 DHT11 LCD1602 I2C
This is my college microprocessor engineering major assignment.
I use kit stm32f103c8t6 as main processor, DHT11 as sensor for measuring temperature and humidity. 1602 LCD display shows measured temperature and humidity.
The system will work as follows:
When power is available the system will be started.
The microprocessor block (STM32F103C8T6) sends a reset signal to the sensor block (DHT11), then the DHT11 measures the temperature and humidity and returns the 5 byte data byte to the microprocessor block. Those 5 bytes of data include 2 bytes of humidity information, 2 bytes of temperature information and 1 byte of test value.
The temperature and humidity values will be displayed on the LCD screen.
If the temperature exceeds the allowed threshold (here I set it to 32 degrees Celsius) the red led will be on and the cooling motor will work, otherwise the green led will be on.
