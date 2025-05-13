# AndroidStudioLoggerTechnique

Kotlin: 
```bash
Log.d("ActivityName", "Current activity: ${this::class.java.simpleName}")
```
```bash
Log.d("ActivityName", "Current activity: ${javaClass.simpleName}")
```

Makefile: 
``` bash
D/ActivityName: Current activity: BirthdayCelebrationActivity
```

Kotlin: 
```bash
Log.d("FragmentInfo", "Current fragment: ${this::class.java.simpleName}")
```
Kotlin: 
```bash
override fun onViewCreated(view: View, savedInstanceState: Bundle?) {
    super.onViewCreated(view, savedInstanceState)

    Log.d("FragmentInfo", "Current fragment: ${this::class.java.simpleName}")
    Log.d("FragmentInfo", "Hosting activity: ${requireActivity()::class.java.simpleName}")
}
```

Makefile: 
``` bash
D/ActivityName: Current activity: BirthdayCelebrationActivity
```

