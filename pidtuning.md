## PID Tuning Notes

* P (proportional) affects how aggressively the FC will act to correct the error, proportional to the magnitude of the error. It is the "right now" factor.  High P manifests as snappy, responsive, unforgiving handling. Low P gives mushy, forgiving handling.
* I (integral) affects how the FC will correct the error based on accumulation of error over time - the "past" factor. Good I tuning will show as attitude stability under throttle changes and external factors (e.g. wind).
* D (derivative) corrects predictively based on the rate of change of the error. It is the "future" factor, which makes rates slow approaching the desired attitude rather than overshooting it.

### General Best Practices

| Best Practice |
| ------------- |
| Tune in Acro mode only |
| Tune each axis separately, starting with P on all axes (with I/D at least halved from default to limit their influence) |

### Solutions

| Symptom | Solutions |
| ------- | ------------------ |
| Bounceback after hard manoeuver | Increase D |
| Hot motors / excessive battery drain | Decrease D |
| Oscillation | Increase D / decrease P |

### Quad Specific Notes

#### Bug Stomper

TODO
