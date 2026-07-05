# ModelBench-ONNX

ModelBench-ONNX is a C++ and Python portfolio project for running, evaluating, and benchmarking ONNX machine learning models.

## Project Goal

The goal of this project is to demonstrate production-style ML inference engineering skills, including:

- Loading ONNX models
- Running inference from C++
- Evaluating model quality
- Measuring latency and throughput
- Reporting results clearly
- Documenting engineering trade-offs

## Planned Features

- C++ command-line inference tool
- ONNX Runtime integration
- Dataset loading
- Accuracy calculation
- Confusion matrix
- Precision, recall, and F1 score
- Average latency
- p50 and p95 latency
- Throughput measurement
- JSON or CSV report output

## Project Structure

```text
ModelBench-ONNX/
├── src/          # C++ source files
├── include/      # C++ header files
├── models/       # ONNX models
├── data/         # Test datasets
├── reports/      # Evaluation and benchmark results
├── docs/         # Design notes and documentation
├── scripts/      # Python helper scripts
├── CMakeLists.txt
├── requirements.txt
└── README.md
