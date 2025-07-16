# First time install
https://www.python.org/downloads/ 

Windows: install from website, not Store

Mac: enable virtual environment
python3 -m venv venv 
. venv/bin/activate
pip install --upgrade bitaxetool
# Download latest firmware
## NerdQAxe
https://github.com/shufps/ESP-Miner-NerdQAxePlus/releases/  
esp-miner-factory-NerdQAxe++-v1.0.31.bin
```wget https://github.com/shufps/ESP-Miner-NerdQAxePlus/releases/download/v1.0.31/esp-miner-factory-NerdQAxe++-v1.0.31.bin -O esp-miner-factory-nerdqaxe.bin```
## Bitaxe
https://github.com/bitaxeorg/ESP-Miner/releases  
esp-miner-factory-401-v2.9.0.bin
```wget https://github.com/bitaxeorg/ESP-Miner/releases/download/v2.9.0/esp-miner-factory-601-v2.9.0.bin -O esp-miner-factory-bitaxe.bin```

# Download latest configuration
```wget https://raw.githubusercontent.com/powerminingio/bitaxe/refs/heads/main/config/Nerdqaxe%2B%2B_config_black_june.csv -O nerdqaxe_config.csv
```
```
wget https://raw.githubusercontent.com/powerminingio/bitaxe/refs/heads/main/config/Bitaxe_config_401_july.csv -O bitaxe_config.csv
```
# Run bitaxetool
```
bitaxetool --firmware <path to the firmware>
bitaxetool --config <path to the config>
```

# Sample command lines:
```
bitaxetool --firmware ./config/esp-miner-factory-NerdQAxe++-v1.0.31.bin
bitaxetool --config ./config/config_black_june.cvs

bitaxetool --firmware ./esp-miner-factory-401-v2.4.2.bin
bitaxetool --config ./config-401.cvs
bitaxetool --config ./config-401.cvs --firmware ./esp-miner-factory-401-v2.4.2.bin
```
