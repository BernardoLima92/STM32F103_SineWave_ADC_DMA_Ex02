# STM32F103_SineWave_ADC_DMA_Ex02
Generating of a sinusoidal signal using PWM as a DAC, in parallel with ADC conversions., and in the last a UART transfer.

Este exemplo é bastante ao mostrado no repositório STM32F103_SineWave_ADC_DMA_Ex01. A diferença é que ao final do código, dentro da função
void HAL_ADC_ConvCpltCallBack(ADC_HandleTypeDef* hadc) foi implementada uma rotina para a realização de uma transferência de dados via UART.

Foi adicionado ao hardware montado no Protoboard um push-button conectado ao PB4. Esse botão foi usado para "ordenar" uma transferência de dados
via UART. Toda vez que o botão é pressionado, uma todo o buffer é transferido após seu completo  preenchimento.

1. Configuração do Clock:

![SW2_Clock](https://user-images.githubusercontent.com/114233216/192543973-e187f06b-bfec-4514-b516-fbee9b8069bb.png)


2. Configuração do TIMER 2:

![SW2_TIM2a](https://user-images.githubusercontent.com/114233216/192544007-030ebe71-8b20-4991-b60f-f1d97421d90d.png)
![SW2_TIM2b](https://user-images.githubusercontent.com/114233216/192544021-73a5dd15-3108-468f-99ab-3d66b0b75dc0.png)


3. Configuração do TIMER 4:

![SW2_TIM4a](https://user-images.githubusercontent.com/114233216/192544072-d70840d3-2af4-42a8-a963-0ee1f3a66054.png)
![SW2_TIM4b](https://user-images.githubusercontent.com/114233216/192544107-ed6a1da8-b5e5-47f2-9e74-31b02e6dc1c8.png)
![SW2_TIM4c](https://user-images.githubusercontent.com/114233216/192544128-85f90f4e-a9c0-4c03-8f5f-d8ad659c63d5.png)



4. COnfiguração do ADC:
![SW2_ADCa](https://user-images.githubusercontent.com/114233216/192544182-fa8469e1-2cb5-4243-adfe-f7d66778996e.png)
![SW2_ADCb](https://user-images.githubusercontent.com/114233216/192544213-f2223acd-9470-499c-8ea9-124dbd858de5.png)


5. Configuração do UART:

![SW2_UART](https://user-images.githubusercontent.com/114233216/192544259-d097ee9b-66be-4d8e-84b9-d5a7b49a8b77.png)


6. COnfiguração do DMA:

![SW2_DMA](https://user-images.githubusercontent.com/114233216/192544505-7170dc1e-7ee6-4df3-b301-bd4b20257612.png)


7. Parte Adicionada ao Código:

![SW2_Code1](https://user-images.githubusercontent.com/114233216/192544564-58d31619-0f55-495d-aeeb-c10b2d4a54b5.png)


8. Circuito Montado na Protoboard:




