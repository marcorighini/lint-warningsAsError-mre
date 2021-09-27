# lint-warningsaserrors-mre
Minimum reproducible error for lint warningsAsErrors with AGP 7.0.2

Running ./gradlew :app:lint finds 2 warnings but they are not escalated to errors.
They should be escalated to errors based on the directive 
```
    lint {
        ...
        warningsAsErrors true
        ...
    }
```
in `app/build.gradle`
