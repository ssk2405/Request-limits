🚀 Kubernetes Resource Requests and Limits – Stress Test Pod
This is a simple demo pod to understand how Kubernetes resource requests and limits work, using a memory stress test.

🧠 What It Does
Runs a container that allocates 80MB of memory for 10 seconds.

Sets:

memory request: 50Mi – the minimum memory guaranteed.

memory limit: 100Mi – the maximum memory allowed.

🎯 Purpose
Test how Kubernetes schedules and manages pods based on memory requests and limits.

Observe OOM (Out of Memory) behavior if limit is exceeded.

How to Apply: kubectl apply -f stress-test.yaml
Clean Up: kubectl delete pod stress-test

