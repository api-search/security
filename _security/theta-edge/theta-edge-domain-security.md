---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: thetaedgecloud.com
  spf: true
hosts:
- cert_expires: Sep 30 03:17:10 2026 GMT
  host: www.thetaedgecloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Theta Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Theta EdgeCloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Theta EdgeCloud
provider_slug: theta-edge
slug: theta-edge-domain-security
source_filename: theta-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thetaedgecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 03:17:10 2026 GMT\n  hsts: false\ndomains:\n- domain: thetaedgecloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theta-edge/refs/heads/main/security/theta-edge-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Distributed Computing
- GPU Compute
- AI Compute
- AI Inference
- AI Training
- Edge Computing
- Video Transcoding
- Live Streaming
- Video API
- Blockchain
- Web3
- Decentralized Infrastructure
- DePIN
- LLM
- Generative AI
- RAG
- NFT
- DRM
- EVM Compatible
- Storage
---
