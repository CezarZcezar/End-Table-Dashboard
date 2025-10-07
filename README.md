# End Table Dashboard
***
## Overview
An End Table Dashboard based on ESP32 with 2.4" display, with 3D printed enclousure. 
## Features
- One button
- SPX40 temperature, humidity sensor
- 2.4 inch TFT display
## Parts used:
- [ESP32 WROOM32 Development Board](aliexpress.com/item/1005006449303342.html?spm=a2g0o.productlist.main.2.408a5d18XLXhDs&algo_pvid=67c871d7-9346-4dc9-802a-fa74fb8653cb&algo_exp_id=67c871d7-9346-4dc9-802a-fa74fb8653cb-1&pdp_ext_f=%7B"order"%3A"1247"%2C"eval"%3A"1"%7D&pdp_npi=6%40dis%21PLN%2117.73%2117.71%21%21%2133.94%2133.90%21%40210385db17573401293181297ed3b6%2112000039288143047%21sea%21PL%211907567941%21X%211%210%21n_tag%3A-29919%3Bd%3A40205d64%3Bm03_new_user%3A-29895&curPageLogUid=7sRO7PUHjNx3&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005006449303342%7C_p_origin_prod%3A)
- [Waveshare 2.4" TFT Dispaly](https://aliexpress.com/item/1005009014044858.html?gatewayAdapt=glo2pol) 
- [DFRobot SHT40 Humidity & Temperature Sensor](https://www.dfrobot.com/product-2437.html?srsltid=AfmBOoq9PaI5Pph8t06wIh6i-qbhoI6mTxdu-A5Ws_bPBEE3pTTctKSM)
- [400 slot breadboard(55 x 83 mm)](https://aliexpress.com/item/1005007085965483.html?spm=a2g0o.productlist.main.35.5b945f67qbIFhg&utparam-url=scene%3Asearch%7Cquery_from%3Apc_back_same_best%7Cx_object_id%3A1005007085965483%7C_p_origin_prod%3A&algo_pvid=c0c148ff-d357-4f85-a8b5-c928aaf3f86d&algo_exp_id=c0c148ff-d357-4f85-a8b5-c928aaf3f86d&pdp_ext_f=%7B%22order%22%3A%222879%22%7D&pdp_npi=6%40dis%21PLN%216.09%216.09%21%21%2111.66%2111.66%21%402103892f17573403143662903ee64a%2112000039350408719%21sea%21PL%211907567941%21X%211%210%21n_tag%3A-29919%3Bd%3A40205d64%3Bm03_new_user%3A-29895)
- [1 momentary push button](https://aliexpress.com/item/4001081730289.html?spm=a2g0o.productlist.main.5.43d71113HnGqL9&algo_pvid=b0b3ad33-151c-4c62-84a3-13139eee3890&algo_exp_id=b0b3ad33-151c-4c62-84a3-13139eee3890-4&pdp_ext_f=%7B%22order%22%3A%222743%22%2C%22eval%22%3A%221%22%7D&pdp_npi=6%40dis%21PLN%217.52%218.63%21%21%212.02%212.32%21%40211b80e117573403428014940ef37c%2110000014240381776%21sea%21PL%211907567941%21X%211%210%21n_tag%3A-29919%3Bd%3A40205d64%3Bm03_new_user%3A-29895&curPageLogUid=eMDkcam72MG5&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A4001081730289%7C_p_origin_prod%3A)
- [Some male-to-female Dupont wires](https://aliexpress.com/item/1005004647016228.html?spm=a2g0o.productlist.main.1.35da75aezGxPwd&algo_pvid=1d4d3d77-f353-4106-b48c-f8fa18bc3b45&algo_exp_id=1d4d3d77-f353-4106-b48c-f8fa18bc3b45-0&pdp_ext_f=%7B%22order%22%3A%223401%22%2C%22eval%22%3A%221%22%7D&pdp_npi=6%40dis%21PLN%215.10%215.10%21%21%211.37%211.37%21%40211b61a417573403873468752ea79d%2112000029976597959%21sea%21PL%211907567941%21X%211%210%21n_tag%3A-29919%3Bd%3A40205d64%3Bm03_new_user%3A-29895&curPageLogUid=R1JLSPnn1TRy&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005004647016228%7C_p_origin_prod%3A) and [some U-shape breadboard wires](https://aliexpress.com/item/1005007175633091.html?spm=a2g0o.productlist.main.2.5a133f29EzGdDS&algo_pvid=81da215d-6534-4948-ae53-f2407d790a36&algo_exp_id=81da215d-6534-4948-ae53-f2407d790a36-1&pdp_ext_f=%7B%22order%22%3A%221924%22%2C%22eval%22%3A%221%22%7D&pdp_npi=6%40dis%21PLN%218.79%218.36%21%21%2116.83%2116.01%21%402103856417573405229388185e75ff%2112000039704758641%21sea%21PL%211907567941%21X%211%210%21n_tag%3A-29919%3Bd%3A40205d64%3Bm03_new_user%3A-29895%3BpisId%3A5000000184800685&curPageLogUid=h0BLbpH93uzy&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007175633091%7C_p_origin_prod%3A)
- 2 M2x3 mm socket screw
% ## Schematic
## Breadboard Connections/Prototype
![image](https://github.com/CezarZcezar/Bed_End_Table_Dashboard/blob/master/Connection_Schematic.png)
## Enclosure
![image](https://github.com/CezarZcezar/Bed_End_Table_Dashboard/blob/master/Images/Enclosure.png)
## Final assembly
![image](https://github.com/CezarZcezar/Bed_End_Table_Dashboard/blob/master/Images/Assembled_View_1.JPEG)
![image](https://github.com/CezarZcezar/Bed_End_Table_Dashboard/blob/master/Images/Assembled_View_2.JPEG)
![image](https://github.com/CezarZcezar/Bed_End_Table_Dashboard/blob/master/Images/Inside_View_1.JPEG)
## Software
## Future
- Add air quality sensors
- Design dedicated PCB
