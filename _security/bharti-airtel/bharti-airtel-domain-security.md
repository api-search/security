---
api_specs:
- filename: bharti-airtel-iq-sms-openapi.yml
  format: yaml
  label: Airtel IQ SMS API
  slug: airtel-iq-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-iq-sms-openapi.yml
- filename: bharti-airtel-iq-reporting-openapi.yml
  format: yaml
  label: Airtel IQ Reporting API
  slug: airtel-iq-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-iq-reporting-openapi.yml
- filename: bharti-airtel-iot-openapi.yml
  format: yaml
  label: Airtel IoT API
  slug: airtel-iot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-iot-openapi.yml
- filename: bharti-airtel-locate-openapi.yml
  format: yaml
  label: Airtel Locate API
  slug: airtel-locate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-locate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airtel.in
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:dmarc29@airteliot.co.in; ruf=mailto:dmarc29@airteliot.co.in; adkim=r; aspf=s; rf=afrf
  dnssec: false
  domain: airteliot.co.in
  note: Added manually; the registrable domain behind the Airtel IoT API host.
  spf: true
  spf_record: v=spf1 include:airtel.com -all
hosts:
- cert_expires: Aug  4 05:02:10 2026 GMT
  host: www.airtel.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: iqsms.airtel.in
  https: false
  note: The Airtel IQ SMS API host (A record 122.187.47.153) refused every anonymous connection during this round (curl exit 28 / 000). It is reachable only from allow-listed enterprise networks, so no TLS or HSTS posture could be recorded. Absence of data here is access control, not a finding about the host's configuration.
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: openapi.airtel.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: m2m.airteliot.co.in
  hsts: false
  https: true
  note: Added manually — the Airtel IoT API host sits on a different registrable domain (airteliot.co.in) than the rest of the estate and was outside the automated probe's host set. It is the only API host in the estate that negotiates TLS 1.2 rather than TLS 1.3, and the only one that returns no Strict-Transport-Security header.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bharti Airtel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bharti Airtel, probed live across 4 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bharti Airtel
provider_slug: bharti-airtel
slug: bharti-airtel-domain-security
source_filename: bharti-airtel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airtel.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 05:02:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: iqsms.airtel.in\n  https: false\n  note: >-\n    The Airtel IQ SMS API host (A record 122.187.47.153) refused every anonymous connection during\n    this round (curl exit 28 / 000). It is reachable only from allow-listed enterprise networks, so\n    no TLS or HSTS posture could be recorded. Absence of data here is access control, not a finding\n    about the host's configuration.\n- host: openapi.airtel.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: m2m.airteliot.co.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\n  note: >-\n    Added manually — the Airtel IoT API host sits on a different\
  \ registrable domain\n    (airteliot.co.in) than the rest of the estate and was outside the automated probe's host set.\n    It is the only API host in the estate that negotiates TLS 1.2 rather than TLS 1.3, and the only\n    one that returns no Strict-Transport-Security header.\ndomains:\n- domain: airtel.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: airteliot.co.in\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:airtel.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:dmarc29@airteliot.co.in; ruf=mailto:dmarc29@airteliot.co.in;\n    adkim=r; aspf=s; rf=afrf\n  note: Added manually; the registrable domain behind the Airtel IoT API host.\nsummary:\n  hosts_probed: 4\n  https: 3\n  hsts: 2\n  dnssec: 0\n  caa: 0\n  spf: 2\n  dmarc: 2\n  gaps:\n  - No DNSSEC on either registrable domain.\n  - No CAA records on either registrable domain — any CA may issue for airtel.in\
  \ or airteliot.co.in.\n  - DMARC is p=quarantine on both, not p=reject.\n  - No HSTS on the Airtel IoT API host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/security/bharti-airtel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- India
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- CPaaS
- Messaging
- SMS
- RCS
- Voice
- IoT
- M2M
- Device Location
- Broadband
- 5G
- Identity Verification
- Carrier Billing
- Consent Management
---
