# Pharo Interface Garden
A place where all C bindings for pharo can hang around, along with its creator, [pharo-cig](https://github.com/pharo-cig/pharo-cig).

## Warning! Install requirements 
We use the last version of UnifiedFFI (that we evolve even while making pharo-cig work).   
If you are using one of the citizens of the garden in a version older than Pharo 14, is highly probably 
you need to first install the compatible version of [UnifiedFFI](https://github.com/pharo-cig/UnifiedFFI)

```smalltalk
Metacello new
	repository: 'github://pharo-cig/UnifiedFFI:v1.1';
	baseline: 'UnifiedFFIFull';
	onConflict: [ :n | n useIncoming ];
	onUpgrade: [ :n | n useIncoming ];
	ignoreImage;
	load.
```

**NOTE:** `v1.0` is a stable tag, use the last release 😄
