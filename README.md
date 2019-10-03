# Vaja4-interrupt-button-STM32F0
<h4>1. Glede na vašo razvojno ploščico in razširitveno vezje s tipkami, izberite ustrezen digitalni vhod kot
interrupt (GPIO_EXT...) in izhod za zeleno LED. Zapišite izbrana pina:</h4>
<p>Pin14,Pin9.
</p>

<h4>2. Znotraj te funkcije zapišite ukaz za vklop/izklop zelene LED (pomagajte si z metodo toggle, glej vaja0a).</h4>
<p>HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_9).</p>

<h4>3. Koliko znaša(v mili sekundah) zapisana zakasnitev?</h4>
<p>10000.</p>

<h4>4. V user code begin 3 - zanka while(1) - zapišite ukaz za utripanje modre LED (metoda toggle, glej vaja0a):</h4>
<p>HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_8).</p>

<h4>5. V to zanko dodajte ukaz za zakasnitev z funkcijo Delay iz knjižnice HAL, in sicer pol sekunde (glej vaja0a)</h4>
<p>HAL_Delay(500).</p>
<h4>6. Opazujte delovanje (utripanje modre LED). Kaj se zgodi, ko pritisnemo na modro tipko na STM32F0?</h4>
<p>Prižge se zelena LED-dioda.</p>

<h4>7. Ali pritisk na modro tipko vpliva na utripanje modre LED in zakaj?</h4>
<p>Ne vpliva, ker v programski kodi ni takšnih ukazov. </p>

<h4>Komentar: LED-dioda deluje na principu pritiska na tipko, ki prižge Zeleno LED-diodo, Modra LED-dioda pa zraven utripa. </h4>











