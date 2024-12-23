# tea standard (Tea24) [work in progress]
[types](#types)  
[declarations](#declarations)

## types

### integer types

#### unsigned

* uint8_t - unsigned 8 bit integer (byte)
* uint16_t - unsigned 16 bit integer (short)
* uint32_t - unsigned 32 bit integer (int)
* uint64_t - unsigned 64 bit integer (long)

#### signed

* int8_t - signed 8 bit integer (byte)
* int16_t - signed 16 bit integer (short)
* int32_t - signed 32 bit integer (int)
* int64_t - signed 64 bit integer (long)

### character types

* char8_t - 8 bit character (ascii)
* char16_t - 16 bit character (unicode)

### other primitive types

* bool - unsigned 8 bit integer that can be 0 (false) or anything else (true)
* void - absolutely nothing (basically only used in function declarations)

## declarations

### declaring variables

#### undefined

`type name;` to initialize an undefined variable  

#### defined

`type name = value;` to define a variable  
`const type name = value;` to define a constant variable  

### declaring arrays

#### undefined

`type[size];` to initialize an undefined array of variable with size  

#### defined

`type[size] = {value1,value2...};` OR `type[size] = "string literal";` to define an array of variable with size  
`const type[size] = {value1,value2...}` OR `const type[size] = "string literal";` to define constant array of type variable with size

### declaring functions

```tea
type name(type arg1, type arg2...)
    return value; // no value if void
end
```



