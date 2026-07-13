---
api_specs:
- filename: ibm-watsonx-ai-openapi.yml
  format: yaml
  label: IBM Watsonx.ai API
  slug: watsonx-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-watsonx-ai-openapi.yml
- filename: ibm-watsonx-assistant-openapi.yml
  format: yaml
  label: IBM Watsonx Assistant V2 API
  slug: watsonx-assistant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-watsonx-assistant-openapi.yml
- filename: ibm-natural-language-understanding-openapi.yml
  format: yaml
  label: IBM Natural Language Understanding API
  slug: natural-language-understanding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-natural-language-understanding-openapi.yml
- filename: ibm-speech-to-text-openapi.yml
  format: yaml
  label: IBM Speech to Text API
  slug: speech-to-text
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-speech-to-text-openapi.yml
- filename: ibm-text-to-speech-openapi.yml
  format: yaml
  label: IBM Text to Speech API
  slug: text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-text-to-speech-openapi.yml
- filename: ibm-cloud-object-storage-openapi.yml
  format: yaml
  label: IBM Cloud Object Storage API
  slug: cloud-object-storage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-cloud-object-storage-openapi.yml
- filename: ibm-kubernetes-service-openapi.yml
  format: yaml
  label: IBM Cloud Kubernetes Service API
  slug: kubernetes-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-kubernetes-service-openapi.yml
- filename: ibm-vpc-openapi.yml
  format: yaml
  label: IBM Cloud VPC API
  slug: vpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-vpc-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ibm.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appdomain.cloud
  spf: false
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: developer.ibm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: cloud.ibm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: s3.us-south.cloud-object-storage.appdomain.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: International Business Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for International Business Machines, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: International Business Machines
provider_slug: international-business-machines
slug: international-business-machines-domain-security
source_filename: international-business-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\n- host: s3.us-south.cloud-object-storage.appdomain.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ibm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: appdomain.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/security/international-business-machines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
---
