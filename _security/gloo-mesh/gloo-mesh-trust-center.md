---
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Gloo Mesh Trust Center
name_suffix: Trust Center
overview: Gloo Mesh maintains a public trust center covering its security and compliance posture.
provider_name: Gloo Mesh
provider_slug: gloo-mesh
slug: gloo-mesh-trust-center
source_filename: gloo-mesh-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://trust.solo.io/\nurl: https://trust.solo.io/\nname: Solo Trust Center\nplatform: Vanta\ncertifications: []\ncertifications_note: >-\n  NONE READABLE — and that is the finding, not an omission. trust.solo.io returns HTTP 200\n  with a 6.6 KB Vanta shell whose entire body renders client-side from\n  assets.vanta.com bundles; the served HTML carries a title, a description and font preloads\n  and no certification, control or subprocessor name. The Vanta public API for the trust\n  center (slug 3wkg6mnjdn7q8adrbhqvzs) answers 401 unauthenticated. So a real trust program\n  exists and a human can read it in a browser, but no machine can read WHICH frameworks it\n  covers. No certification is asserted here and no `Compliance` pointer is emitted on the\n  strength of it — asserting SOC 2 or ISO 27001 because a Vanta page exists would be a guess.\nx-evidence:\n  fetched: '2026-09-12'\n  url: https://trust.solo.io/\n  http_status:\
  \ 200\n  content_type: text/html\n  bytes: 6595\n  rendering: client-side (Vanta trust report bundle)\n  vanta_slug: 3wkg6mnjdn7q8adrbhqvzs\n  api_probe:\n    url: https://api.vanta.com/v1/public/trust-center/3wkg6mnjdn7q8adrbhqvzs\n    http_status: 401\nrelated:\n  security_policy: https://www.solo.io/security\n  cve_lifecycle: https://docs.solo.io/gloo-mesh-enterprise/latest/reference/security_updates/cve-lifecycle\n  vulnerability_disclosure: security/gloo-mesh-vulnerability-disclosure.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gloo-mesh/refs/heads/main/security/gloo-mesh-trust-center.yml
summary_line: trust center published
tags:
- Istio
- Kubernetes
- Multi-Cluster
- Open Source
- Service Mesh
- Envoy
- Kubernetes CRDs
- Protobuf
- Policy Enforcement
- Observability
trust_url: https://trust.solo.io/
---
