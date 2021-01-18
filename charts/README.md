# Smoketest


helm upgrade \
  --create-namespace \
  --install \
  --wait \
  --namespace=open5gs \
  "udm" \
  "$(git rev-parse --show-toplevel)/charts/udm"