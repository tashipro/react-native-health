# getLatestSteps

Returns total steps of latest date available in Apple Health Kit.

This function most probably used to check whether Apple Health Kit has steps data or not. If not then it will return the error and based on the native error, it can be managed on react native. This function can be used at permission time.

Example input options:

```javascript
const options = { unit: 'count' }
```

Call the method:

```javascript
AppleHealthKit.getLatestSteps(
  (options: HealthInputOptions),
  (err: Object, results: HealthValue) => {
    if (err) {
      return
    }
    console.log(results)
  },
)
```

Example output:

```json
{
  "endDate": "2021-11-10T12:00:00.000+0530",
  "startDate": "2021-11-10T12:00:00.000+0530",
  "value": 123,
}
```
