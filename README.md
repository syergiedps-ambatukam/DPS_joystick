# 🕹️ DPS_joystick

        +-------------------+      +-------------------+    +--------------------------+  
        | 1.DPS Joystick    | ->   |  2. PC DPS        | -> | 3. Panel DPS             |
        +--------+----------+      +--------+----------+    +--------+-----------------+

Update pada coding sebelumnya

| sebelum | sesudah | alasan perubahan |
|--------------|------------|------------------------|
|Steaming data per 0.5 detik posisi joystick | Kirim data hanya ketika ada perubahan/instruksi | Memperingan kerja microcontroller dan membuat responsif |
| Timer Triggered | Event Triggered | Metode yang cocok untuk mengakomodir yang dibutuhkan |

Pinout Joystick
| Tombol | Pin Arduino |
|--------------|------------|
|steering 1 Left | 2 |
|steering 1 Right | 3 |
| Slider 1 | A1 |
|steering 2 Left | 6 |
|steering 2 Right | 7 |
| Slider 2 | A2 |
|steering 3 Left | 23 |
|steering 3 Right | 9 |
| Slider 3 | A3 |
|steering 4 Left | 12 |
|steering 4 Right | 19 |
| Slider 4 | A4 |


Arduino Library Requirements
- pubsubclient by nick o lerry ver 2.8

- Ethernet by Various Author ver 2.0.2
