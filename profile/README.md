# Pharo Interface Garden
A place where all C bindings for pharo can hang around, along with its creator, [pharo-cig](https://github.com/pharo-cig/pharo-cig).

## Warning! Install requirements 
We use the last version of UnifiedFFI (that we evolve even while making pharo-cig work).   
If you are using one of the citizens of the garden in a version older than Pharo 14, is highly probably 
you need to first install the compatible version of [UnifiedFFI](https://github.com/pharo-cig/UnifiedFFI)

```smalltalk
Metacello new
	repository: 'github://pharo-cig/UnifiedFFI:stable';
	baseline: 'UnifiedFFIFull';
	onConflict: #useIncoming;
	onUpgrade: #useIncoming;
	ignoreImage;
	load.
```

**NOTE:** `stable` is a moving tag that points to the latest stable release.
