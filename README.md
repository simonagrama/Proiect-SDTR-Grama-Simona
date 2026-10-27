Proiect SDTR Grama Simona SECI-RCD anul 1

**Titlu:** Sistem distribuit de monitorizare și de control în timp real al unui ventilator în funcție de temperatură, bazat pe STM32, FreeRTOS și CAN 

**Descriere:** Proiectul constă într-o aplicație embedded distribuită, bazată pe un microcontroller, care monitorizează temperatura și reglează în timp real viteza unui ventilator în funcție de temperatura măsurată. Microcontrollerul vizat este STM32 Nucleo-F446RE (ARM Cortex-M4), iar sistemul de operare de timp real folosit este FreeRTOS. Temperatura este achiziționată prin ADC (cu DMA), iar ventilatorul este comandat prin PWM generat de un timer hardware. Aplicația conține două task-uri independente: un task periodic de timp real (prelucrare locală și comanda ventilatorului) și un task de comunicație care implementează stiva de nivel înalt a protocolului, sincronizate prin cozi de mesaje și semafoare. Protocolul de comunicație folosit este CAN, cu controllerul integrat în microcontroller. Al doilea nod din rețea este un adaptor USB-CAN conectat la un laptop. Proiectul include și o analiză a performanțelor de timp real (jitter, latență eveniment-răspuns).

**Link Repository Git:** https://github.com/simonagrama/Proiect-SDTR-Grama-Simona
