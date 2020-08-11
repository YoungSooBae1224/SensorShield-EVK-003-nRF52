*ROHM Sensor Shield

- Applicable Part Number: SensorShield-EVK-003
    ROHM Sensor Shield include sensor
1. BM1383AGLV
2. BH1790GLC with I2C
3. BD1020HFV
4. BD7411G

- Bluetooth Low Energy Chip
    nRF52832
Test Board
1. nRF52DK
2. Lapis - MK71521EK1A

- Change circuit
1. nRF52DK

Change VDD circuit on SensorShield-EVK-003

    remove Pull up resister(R10 and R11).
    
    Connect VDD on nRF52DK and I2C power of the removed pull up resisiter(R10 and R11) SensorShield-EVK-003

2. MK71521EK1A

    Cut SB_P26 and SB_P27.

- Ohter
1. Download SDK15.3 in nordicsemi.com 

    After updating all sensors, I plan to update in the next version.

    https://www.nordicsemi.com/Products/Low-power-short-range-wireless/nRF52832/Download#infotabs

2. Create a ROHM_EVK_003 folder and git pull it in the created folder.

    location : SDK15_directory\examples\ROHM_EVK_003\

3. Lapis - MK71521EK1A

    Please perpare nRF52DK(Need SWD cable for connection) or J-Link debugger. MK71521EK1A is no built-in debugger.
