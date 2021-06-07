# MicroPython_SRAM
基于micropython的外部sram

## 🚀使用

```python
>>>from fsmc import fsmc_sram_buffer
>>>sram_b = fsmc_sram_buffer(5000,0x68000000,0x68000000,0x68000000+0x1388,0x02) # 5000 16bit locations = 10KB
>>>sram_b.write(0x1234)  # 0x1234=4660
>>>sram_b.read_i(0)
4660
```

