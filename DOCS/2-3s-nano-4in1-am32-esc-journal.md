# 2-3s Nano 4in1 AM32 ESC  — Journal Export

- Exported at: 2026-05-30T12:08:03Z
- Project ID: 1885
- Entries: 17

## Entry 1
- ID: 1891
- Author: NAFI
- Created At: 2026-04-12T09:48:39Z

### Content

I started this project, but don't dont know why ;) This will be a 4-in-1 esc. oh! I can use this in my HACK FLY drone. The drone will be fully custom-made.

First, I go to the AM32 documentation and find that it works with many MCUs. So I need to select one.
![image.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDAyNywicHVyIjoiYmxvYl9pZCJ9fQ==--408ef51c4233c931afef680a6b71de65fa554c8b/image.png)

After some research, I chose AT32F421G8U7 because it comes with a QFN-24 package. the smallest of them. 

I also need all of the components to be as small as possible. My PCB size budget is only 25*25mm.

At first, I want to use a 2*2mm size n-channel MOSFET, but those are not available on Aliexpress. So I switched to 3*3mm
![Screenshot 2026-04-12 152702.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDAyOCwicHVyIjoiYmxvYl9pZCJ9fQ==--8b2c469fa369779855d54bd8a8c0ab7faceb6cd9/Screenshot 2026-04-12 152702.png)
 I also used a very small gate driver, DVR8300N(also QFN-24)
![Screenshot 2026-04-12 152627.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDAyOSwicHVyIjoiYmxvYl9pZCJ9fQ==--9c7a23fecbb319b5e72996c8b44b6af77c76fefc/Screenshot 2026-04-12 152627.png)
After placing the main ICs, I routed some connections in the schematic. That's it.
![image.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDAzMCwicHVyIjoiYmxvYl9pZCJ9fQ==--de187f309a13e24c6b2c5d031433fabaa065bc49/image.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/Joe-1cWgr59x/timelapse-Joe-1cWgr59x.mp4

## Entry 2
- ID: 1953
- Author: NAFI
- Created At: 2026-04-12T20:36:31Z

### Content

Just completed the schematic single ESC. 
![Screenshot 2026-04-12 152613.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDE2MiwicHVyIjoiYmxvYl9pZCJ9fQ==--355f9686e31fe2644b21c4045ebc6ba821de8386/Screenshot 2026-04-12 152613.png)
Also, fix a big problem, at first I chose drv8300n QFN-24, which does not come with bootstrap diode. I thought there was no D version of the qfn-24 package. But after searching on Google, I found out that Ti has a version of drv8300D. And it is also available on AliExpress :)

![image.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDE2NCwicHVyIjoiYmxvYl9pZCJ9fQ==--1e055f8fa908650f08dfb76cf023a7a1c444ba4f/image.png)
![Screenshot 2026-04-12 165951.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDE2NSwicHVyIjoiYmxvYl9pZCJ9fQ==--5569a5994207e54ada6b8ceb0665bd8d318d099c/Screenshot 2026-04-12 165951.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/6GfyzV2vDIhM/timelapse-6GfyzV2vDIhM.mp4

## Entry 3
- ID: 2207
- Author: NAFI
- Created At: 2026-04-14T17:34:22Z

### Content

Today I did something very frustrating. Adding 4 same circuit schematics to take u 4in1 ESC.

![Screenshot 2026-04-12 232327.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDY3OSwicHVyIjoiYmxvYl9pZCJ9fQ==--03c617e3eef739847820117ab6326634a1e6fb11/Screenshot 2026-04-12 232327.png)

But here is the catch: I have to manually type and edit every single net pad to its corresponding ESC number (like sda1, sda2, sda3 ...).

![Screenshot 2026-04-12 231841.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDY4MCwicHVyIjoiYmxvYl9pZCJ9fQ==--68f07b1aee05c0cc49387392cf52684844cb782b/Screenshot 2026-04-12 231841.png) 

![Screenshot 2026-04-12 232309.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDY4MSwicHVyIjoiYmxvYl9pZCJ9fQ==--dbccd4061d45e703162e581c4ae425872d42babe/Screenshot 2026-04-12 232309.png)

It took me more than 1 hour to do ;(
But after all the work is done.



### Recording Links

- https://public.lapse-hackclub.link/timelapses/en4dqctDFa-q/timelapse-en4dqctDFa-q.mp4

## Entry 4
- ID: 2354
- Author: NAFI
- Created At: 2026-04-15T18:27:51Z

### Content

So there are too many resistors and capacitors to place in a 2 sided PCB, only 30*30mm. 
![Screenshot 2026-04-12 234142.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDkzMiwicHVyIjoiYmxvYl9pZCJ9fQ==--94a0737f586f5eb01936e47a6dd0c8ed39e53aad/Screenshot 2026-04-12 234142.png)
But somehow I need to do it, so begin with gate drivers and MCUs in diffarent side of the PCB. MCUs on top and gate drivers at the bottom.
![Screenshot 2026-04-13 003505.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDkzNCwicHVyIjoiYmxvYl9pZCJ9fQ==--2775d7c71fa99d0066b990122357b0c423ee6209/Screenshot 2026-04-13 003505.png)
then i stared placing feedback resistors...........


### Recording Links

- https://public.lapse-hackclub.link/timelapses/904tiRd4TA7I/timelapse-904tiRd4TA7I.mp4

## Entry 5
- ID: 2358
- Author: NAFI
- Created At: 2026-04-15T18:43:39Z

### Content

So I started placing gate resistors yesterday, and today it's complete. 


But here is a catch: I placed all gate drivers on one side. For that, all the gate resistors should be on that side too. And for this reason, I created this resistor mesh.
![Screenshot 2026-04-13 180920.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDk0MywicHVyIjoiYmxvYl9pZCJ9fQ==--969a294786c5c6e83d1a3a139c347cf43f45e60f/Screenshot 2026-04-13 180920.png)

Now there is too little space to route all the traces. If I use too many vias, the trace resistance will be greater than the actual resistor value. So I need an efficient way to place all the components........

### Recording Links

- https://public.lapse-hackclub.link/timelapses/mJ234j6gotP4/timelapse-mJ234j6gotP4.mp4

## Entry 6
- ID: 2477
- Author: NAFI
- Created At: 2026-04-16T19:34:21Z

### Content

I switched the placement strategy. 

Instead of placing gate drivers on one side and MCUs on the other, I placed 2 MCUs and 2 gate drivers on one side and the other 2 on the other side.
![Screenshot 2026-04-14 124223.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTE4OCwicHVyIjoiYmxvYl9pZCJ9fQ==--01994eba90963c1cec0e7b20a2947525702ddbf9/Screenshot 2026-04-14 124223.png)


It will significantly reduce the use of more vias and save some space. Accually i got this idea from Kiss Ultra v3 esc.

Also i moved the phase output pad to the edge for edge plating. For this, it can now output more current than a normal multilayer pad.


![Screenshot 2026-04-14 133220.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTE4NywicHVyIjoiYmxvYl9pZCJ9fQ==--97f27e1296822db1e0af18aafb8eab1151b58405/Screenshot 2026-04-14 133220.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/D78rtctXlnH5/timelapse-D78rtctXlnH5.mp4

## Entry 7
- ID: 2741
- Author: NAFI
- Created At: 2026-04-18T17:15:43Z

### Content

Just add the multi layer pads for motor phase output and 2 big pads for power input. And placed them at the board outline for making them castellated holes. I also extend the board outline by 1mm at the pads.
![1000040280.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTc0NCwicHVyIjoiYmxvYl9pZCJ9fQ==--23c94b4bd2d889461b7fbf4f46a6741572d3d1f6/1000040280.png)

And add many vias for high corrent flow.
![1000040282.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTc0OCwicHVyIjoiYmxvYl9pZCJ9fQ==--d9d2a9bf8110f59063407d786d3a40f16fa121d2/1000040282.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/qbsJZ9rIreRg/timelapse-qbsJZ9rIreRg.mp4

## Entry 8
- ID: 2745
- Author: NAFI
- Created At: 2026-04-18T17:39:50Z

### Content

After placing all the pads for castellated holes, I started routing traces. i used 0.18mm trace for all the signal connections. and some 0.2mm.
![Screenshot 2026-04-14 173357.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTc1MywicHVyIjoiYmxvYl9pZCJ9fQ==--6f703c2d31f18603d6cf7ee2cc0c6e5df262895c/Screenshot 2026-04-14 173357.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/uukYo2lN7eIS/timelapse-uukYo2lN7eIS.mp4

## Entry 9
- ID: 2931
- Author: NAFI
- Created At: 2026-04-19T18:57:41Z

### Content

Tracing the 106 signal and the back EMF line is a little bit tricky. But somehow I pulled them off.

![Screenshot 2026-04-20 005207.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NjExMiwicHVyIjoiYmxvYl9pZCJ9fQ==--81688ab64eb48c62890bfc3add05b2f21763113a/Screenshot 2026-04-20 005207.png)

I placed lots of vias of 0.3mm drill hole and 0.5mm diameter, because JLCPCB didn't charge extra for epoxy filled via s if via>0.5mm.


### Recording Links

- https://public.lapse-hackclub.link/timelapses/J-ME_Ey1Y9RK/timelapse-J-ME_Ey1Y9RK.mp4

## Entry 10
- ID: 3239
- Author: NAFI
- Created At: 2026-04-21T17:23:45Z

### Content

Ahh! After many days of work, the PCB routing is finally done (Almost).
![Screenshot 2026-04-17 003909.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NjczNywicHVyIjoiYmxvYl9pZCJ9fQ==--457f48b69e117af58f0583978d9510206b1ab8ab/Screenshot 2026-04-17 003909.png)

The only thing left is to connect some gnd pad to gnd and 3.3v to the main 3.3v pad. But there is no free space left for it.
![Screenshot 2026-04-21 232250.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NjczOCwicHVyIjoiYmxvYl9pZCJ9fQ==--8064693ff0e512f25ccf7be36d65bdd6b732933f/Screenshot 2026-04-21 232250.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/Z7C_Ijw4qDf0/timelapse-Z7C_Ijw4qDf0.mp4

## Entry 11
- ID: 8162
- Author: NAFI
- Created At: 2026-05-20T14:55:40Z

### Content

I just don't have enough space in the PCB to place the 3.3v vias. So i just unrouted the existing routes and created some space to place some 3.3v vias.
![Screenshot 2026-05-19 010940.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTc4NDUsInB1ciI6ImJsb2JfaWQifX0=--c9c2daa076832f5f490210280cda219407c68ce0/Screenshot 2026-05-19 010940.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/LJ-o1sSxgkMX/timelapse-LJ-o1sSxgkMX.mp4

## Entry 12
- ID: 8335
- Author: NAFI
- Created At: 2026-05-21T17:19:05Z

### Content

Finally, I figured out how to place 3.3V vias and route the V+ bus to the DRV8300 gate driver.

![Screenshot 2026-05-20 212708.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTgyMzEsInB1ciI6ImJsb2JfaWQifX0=--1a67eed05e2fdcecdac839cdc9fe3c6b62076174/Screenshot 2026-05-20 212708.png)

![Screenshot 2026-05-20 212723.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTgyMzIsInB1ciI6ImJsb2JfaWQifX0=--4ef7f5c44eed66ccb8f1a9870878d6f292eba02f/Screenshot 2026-05-20 212723.png)

Also added Current sensing, i sued a 2512 size 1mohm sunt resistor and INA180A.

![Screenshot 2026-05-21 090557.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTgyMjksInB1ciI6ImJsb2JfaWQifX0=--99a2e4c0ad3361595722344801a0e7e5e580e82a/Screenshot 2026-05-21 090557.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/t9gTDaKhCvt0/timelapse-t9gTDaKhCvt0.mp4

## Entry 13
- ID: 8481
- Author: NAFI
- Created At: 2026-05-22T15:24:24Z

### Content

Re-configured some connections. Also added some power vias for each phase output and routed some un-routed traces
![Screenshot 2026-05-21 032839.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTg1MzksInB1ciI6ImJsb2JfaWQifX0=--0537a05731e68a41418d4392211a0bc112991b84/Screenshot 2026-05-21 032839.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/GTc06x4hLAUN/timelapse-GTc06x4hLAUN.mp4

## Entry 14
- ID: 9669
- Author: NAFI
- Created At: 2026-05-27T15:28:11Z

### Content

I just need to add some finishing touches. the the pcb design will be completed. 
![Screenshot 2026-05-21 140224.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjE0NTcsInB1ciI6ImJsb2JfaWQifX0=--49a98a4eb590395fd5df7ba74c3de5f6f497284d/Screenshot 2026-05-21 140224.png) i also run some drc cheack in jlcpcb fabricalion web.
![Screenshot 2026-05-21 144235.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjE0NTgsInB1ciI6ImJsb2JfaWQifX0=--2ae39c485cf06991b3194cbc1f02ea74f8dff460/Screenshot 2026-05-21 144235.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/egjknMwtG9es/timelapse-egjknMwtG9es.mp4

## Entry 15
- ID: 10268
- Author: NAFI
- Created At: 2026-05-29T22:53:52Z

### Content

Added the last finishing touch before exporting the production files. Here's the final result
![Screenshot 2026-05-21 110434.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjMyODgsInB1ciI6ImJsb2JfaWQifX0=--f3033cdf4a72822a64dddc63452068848993aeaf/Screenshot 2026-05-21 110434.png)
I tried to make a heat sink CAD model in Onshape, but my pc cant handel the pcb 3d file that why the lapse is 70% blank.


### Recording Links

- https://public.lapse-hackclub.link/timelapses/uD8Hmfb5TllP/timelapse-uD8Hmfb5TllP.mp4

## Entry 16
- ID: 10280
- Author: NAFI
- Created At: 2026-05-30T00:30:34Z

### Content

Completed the Zine design. I'm just out of creativity for designing the zine. 
![Your paragraph text.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjMzMDksInB1ciI6ImJsb2JfaWQifX0=--d8e306e512f59d607a34015ac4411f8cb6b62fd8/Your paragraph text.png)
also 70% completed editing the repo. The only left is to finish making the BOM file. Then the project will be ready to ship.


### Recording Links

- https://public.lapse-hackclub.link/timelapses/k5HC4egpIGsT/timelapse-k5HC4egpIGsT.mp4

## Entry 17
- ID: 10291
- Author: NAFI
- Created At: 2026-05-30T02:07:23Z

### Content

Finally, all done. This will be the lowest cost project i ever done. especially the MCU at32f421 5pcs only cost 3$ thats only 0.75$ each. 
![Screenshot 2026-05-29 205400.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjMzMjUsInB1ciI6ImJsb2JfaWQifX0=--b2d4707d22279af00bc0eafaeac785e2c7f59d2b/Screenshot 2026-05-29 205400.png) Also, the 6-layer PCB with 1u gold plating+ via in pad only 2.45$ beacuse jlcpcb give free epoxy capped via, it via size> 0.5mm.
![Screenshot 2026-05-29 204812.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjMzMjcsInB1ciI6ImJsb2JfaWQifX0=--0350e30e3f5b3982194b0b7c4e4a5de9f8324aea/Screenshot 2026-05-29 204812.png)
I forgot to journal a lapse before, so I am attaching that with it:)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/TJhr2Z3ZKI5y/timelapse-TJhr2Z3ZKI5y.mp4
- https://public.lapse-hackclub.link/timelapses/v6uv_6NIaZKS/timelapse-v6uv_6NIaZKS.mp4
