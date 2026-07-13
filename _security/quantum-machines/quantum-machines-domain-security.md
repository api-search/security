---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: quantum-machines.co
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:infrastructure-staff@python.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pypi.org
  spf: true
hosts:
- cert_expires: Sep 26 08:42:13 2026 GMT
  host: www.quantum-machines.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 19:33:18 2026 GMT
  host: docs.quantum-machines.co
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantum Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantum Machines, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Quantum Machines
provider_slug: quantum-machines
slug: quantum-machines-domain-security
source_filename: quantum-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quantum-machines.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:42:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.quantum-machines.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 19:33:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quantum-machines.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pypi.org\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:infrastructure-staff@python.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantum-machines/refs/heads/main/security/quantum-machines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Quantum Computing
- Quantum Control
- Pulse Level Programming
- QUA
- OPX
- OPX1000
- QOP
- Quantum Orchestration Platform
- Pulse Processing Unit
- Real Time Feedback
- Arbitrary Waveform Generation
- Superconducting Qubits
- Trapped Ions
- Neutral Atoms
- Color Centers
- Cryogenic Electronics
- Hardware
- Israel
---
