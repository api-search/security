---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orthanc-server.com
  spf: true
hosts:
- cert_expires: Jan 10 01:22:02 2027 GMT
  host: www.orthanc-server.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orthanc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orthanc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Orthanc
provider_slug: orthanc
slug: orthanc-domain-security
source_filename: orthanc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orthanc-server.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 01:22:02 2027 GMT\n  hsts: false\ndomains:\n- domain: orthanc-server.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orthanc/refs/heads/main/security/orthanc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- DICOM
- Medical Imaging
- Open Source
- REST API
---
