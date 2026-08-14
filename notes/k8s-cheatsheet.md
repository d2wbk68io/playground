# Kubernetes Quick Ref

- `kubectl get pods -o wide` — show node IPs
- `kubectl logs -f deploy/name --since=5m`
- `kubectl rollout restart deploy/name`
- `kubectl port-forward svc/svc-name 8080:80`
- `kubectl exec -it pod-name -- /bin/sh`
- `kubectl top nodes` — resource usage

## Common YAML gotchas
- Indent with spaces, not tabs
- `kind` and `apiVersion` are case-sensitive
- Use `--dry-run=client -o yaml` to scaffold