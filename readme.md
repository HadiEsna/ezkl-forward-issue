EZKL forward issue

```bash
ezkl gen-circuit-params --calibration-target accuracy --model network.onnx --circuit-params-path ./circuit.json -K 23 -B 22 -S 8
```

```bash
ezkl forward -M network.onnx -D input.json -O input-forwarded.json --circuit-params-path circuit.json
```