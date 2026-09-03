---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: veratech.es
  spf: true
hosts:
- host: veratech.es
  hsts: null
  https: true
  server: Apache
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- host: www.veratech.es
  hsts: null
  https: true
  tls_cert_error: 'openssl verify return code 21: unable to verify the first certificate'
- host: linkehr.veratech.es
  hsts: null
  https: true
  server: Apache
  tls_cert_error: 'openssl verify return code 21: unable to verify the first certificate'
- host: docpeset.veratech.es
  hsts: null
  https: true
  note: Serves a distinct GoDaddy-issued certificate (CN=docpeset.veratech.es) with a COMPLETE chain, unlike the wildcard hosts. This is the control that proves the finding below is a per-host misconfiguration and not a fault in the probing client.
  tls_cert_error: null
kind: domain-security
layout: security
method: probed
name: Veratech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veratech for Health, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Veratech for Health
provider_slug: veratech
slug: veratech-domain-security
source_filename: veratech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py) plus hand-run\n  openssl s_client and curl HEAD probes of the additional Veratech-controlled hosts\n  discovered via certificate transparency\nhosts:\n- host: veratech.es\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n  server: Apache\n- host: www.veratech.es\n  https: true\n  tls_cert_error: 'openssl verify return code 21: unable to verify the first certificate'\n  hsts: null\n- host: linkehr.veratech.es\n  https: true\n  tls_cert_error: 'openssl verify return code 21: unable to verify the first certificate'\n  hsts: null\n  server: Apache\n- host: docpeset.veratech.es\n  https: true\n  tls_cert_error: null\n  hsts: null\n  note: >-\n    Serves a distinct GoDaddy-issued certificate (CN=docpeset.veratech.es) with a COMPLETE\n    chain,\
  \ unlike the wildcard hosts. This is the control that proves the finding below is a\n    per-host misconfiguration and not a fault in the probing client.\ndomains:\n- domain: veratech.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nfindings:\n- id: incomplete-tls-chain\n  severity: medium\n  hosts:\n  - veratech.es\n  - www.veratech.es\n  - linkehr.veratech.es\n  detail: >-\n    All three hosts present the wildcard leaf CN=*.veratech.es issued by\n    \"C=ES, O=Soluciones Corporativas IP SL, CN=Don Dominio RSA DV SSL CA 2\" but do NOT send\n    that intermediate in the handshake. openssl reports verify return code 21 (\"unable to\n    verify the first certificate\") and Python's ssl reports CERTIFICATE_VERIFY_FAILED.\n  impact: >-\n    Browsers usually recover by fetching the missing intermediate via the AIA extension, so a\n    human visitor sees nothing wrong. Strict clients do not: this pipeline's own WebFetch\n    failed against https://veratech.es/\
  \ with \"unable to verify the first certificate\", and\n    Java, Python requests, curl without AIA, and most agent HTTP stacks will fail the same\n    way. For a company whose product is Java-based and whose buyers are hospital IT\n    departments running strict TLS, this is the single most consequential technical defect\n    found on the public surface.\n  verified: '2026-09-02'\n  control: >-\n    docpeset.veratech.es, on the same parent domain, validates cleanly — the client is fine,\n    the wildcard hosts' chain is not.\n  remediation: >-\n    Concatenate the \"Don Dominio RSA DV SSL CA 2\" intermediate into the certificate file the\n    Apache SSLCertificateFile / SSLCertificateChainFile directive serves.\n- id: no-hsts\n  severity: low\n  hosts:\n  - veratech.es\n  - linkehr.veratech.es\n  detail: No Strict-Transport-Security header is returned by any Veratech host.\n  verified: '2026-09-02'\n- id: no-dnssec\n  severity: low\n  domain: veratech.es\n  detail: DNSSEC is not enabled\
  \ on veratech.es.\n  verified: '2026-09-02'\n- id: no-caa\n  severity: low\n  domain: veratech.es\n  detail: >-\n    No CAA record is published, so any public CA may issue for veratech.es and its\n    subdomains.\n  verified: '2026-09-02'\n- id: dmarc-policy-none\n  severity: low\n  domain: veratech.es\n  detail: >-\n    SPF and DMARC records both exist — better than most of this cohort — but the DMARC policy\n    is p=none, which reports on spoofing without rejecting it. Notable for a company that\n    solicits contact by email (contacto@veratech.es, veratech@veratech.es) from hospital\n    staff.\n  verified: '2026-09-02'\n- id: research-tools-on-ad-hoc-infrastructure\n  severity: informational\n  detail: >-\n    Several veratech.es subdomains redirect off the corporate estate to unmanaged endpoints\n    over PLAINTEXT HTTP — snquery.veratech.es 301s to http://biohub.nethits.com:51562/snquery,\n    nerplus.veratech.es and documentalista.veratech.es 301s to\n    http://veratechnas1.synology.me\
  \ (a consumer Synology DDNS name, one on port 9999), and\n    openehr2fhir.veratech.es resolves through to http://141.147.80.147:8080/openehr2fhir/.\n    These are research and demo tools, not production services, but the redirects downgrade\n    from HTTPS to HTTP and land on hosts outside the certificate estate.\n  verified: '2026-09-02'\nsubdomain_discovery:\n  method: certificate transparency (crt.sh)\n  hosts_found:\n  - confluence.veratech.es\n  - ctmap.veratech.es\n  - ctmap2.veratech.es\n  - docpeset.veratech.es\n  - documentalista.veratech.es\n  - help.veratech.es\n  - jira.veratech.es\n  - nerplus.veratech.es\n  - notify.veratech.es\n  - openehr2fhir.veratech.es\n  - snquery.veratech.es\n  - veratech.es\n  - www.veratech.es\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veratech/refs/heads/main/security/veratech-domain-security.yml
summary_line: DMARC
tags:
- Company
- Healthcare
- Health Data
- Semantic Interoperability
- openEHR
- HL7 FHIR
- ISO 13606
- SNOMED CT
- OMOP CDM
- Clinical Data
- Electronic Health Records
- Consulting
- Spain
---
