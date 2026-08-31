---
api_specs:
- filename: cosmose-ai-contact-form-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Contact Form Controller API
  slug: cosmose-ai-contact-form-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-contact-form-controller-api-openapi.yml
- filename: cosmose-ai-crucible-token-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Crucible Token Controller API
  slug: cosmose-ai-crucible-token-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-crucible-token-controller-api-openapi.yml
- filename: cosmose-ai-forget-me-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Forget Me Controller API
  slug: cosmose-ai-forget-me-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-forget-me-controller-api-openapi.yml
- filename: cosmose-ai-invitation-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Invitation Controller API
  slug: cosmose-ai-invitation-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-invitation-controller-api-openapi.yml
- filename: cosmose-ai-kkn-onboarding-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Kkn Onboarding Controller API
  slug: cosmose-ai-kkn-onboarding-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-kkn-onboarding-controller-api-openapi.yml
- filename: cosmose-ai-learn-to-code-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Learn To Code Controller API
  slug: cosmose-ai-learn-to-code-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-learn-to-code-controller-api-openapi.yml
- filename: cosmose-ai-merchant-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Merchant Controller API
  slug: cosmose-ai-merchant-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-merchant-controller-api-openapi.yml
- filename: cosmose-ai-newsletter-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Newsletter Controller API
  slug: cosmose-ai-newsletter-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-newsletter-controller-api-openapi.yml
- filename: cosmose-ai-onboarding-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Onboarding Controller API
  slug: cosmose-ai-onboarding-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-onboarding-controller-api-openapi.yml
- filename: cosmose-ai-registration-admin-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Registration Admin Controller API
  slug: cosmose-ai-registration-admin-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-registration-admin-controller-api-openapi.yml
- filename: cosmose-ai-registration-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Registration Controller API
  slug: cosmose-ai-registration-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-registration-controller-api-openapi.yml
- filename: cosmose-ai-school-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI School Controller API
  slug: cosmose-ai-school-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-school-controller-api-openapi.yml
- filename: cosmose-ai-token-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Token Controller API
  slug: cosmose-ai-token-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-token-controller-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cosmose.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cosmose.co
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: cosmose.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 02:35:59 2026 GMT
  host: api.sg.cosmose.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cosmose Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosmose AI, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cosmose AI
provider_slug: cosmose-ai
slug: cosmose-ai-domain-security
source_filename: cosmose-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cosmose.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n- host: api.sg.cosmose.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:35:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cosmose.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: cosmose.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/security/cosmose-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail Intelligence
- offline-analytics
- Location Intelligence
- AdTech
- consumer-behavior
- Shopper Analytics
- Mobile SDK
- Advertising
- Artificial Intelligence
- Singapore
---
