# Smile Confidence Quiz (Reflections Dental Group)

Self-hosted lead-gen quiz for Reflections Dental Group, Calgary. Single static page,
no build step. Leads POST to the `reflections-quiz-relay` Cloudflare Worker, which
stores every submission and forwards to the practice CRM once a webhook is configured.

**This is a client project, separate from the Kaizen quiz fleet.**

- Live page: https://jameson-kaizen.github.io/reflections-smile-quiz/
- Ops doc: `SELF-HOST.md` in the project folder (not this repo)

To move this page to another host later, copy `index.html`. To re-point lead
delivery, set `WEBHOOK_URL` on the Worker and redeploy. No page changes needed.
