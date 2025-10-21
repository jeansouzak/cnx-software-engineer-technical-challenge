# Technical Challenge — Software Engineer

**Focus:** quality of process and decisions (requirements understanding, architecture, implementation, reliability)

**Suggested timeline:** 7 days

## Objective

Build a service that reads a **CSV mailing list** and triggers **e-mail sends** using an **authenticated sending API**.

* **Email subject:** *Complete your registration*
* **Email body:** *Thank you for signing up. Please verify your token {token} to continue.*
* **{token}:** must be generated randomly per recipient.

## API Information

**Base URL:** `https://email-test-api-475816.ue.r.appspot.com`

**Documentation:**
* Swagger UI: https://email-test-api-475816.ue.r.appspot.com/docs
* ReDoc: https://email-test-api-475816.ue.r.appspot.com/redoc
* OpenAPI Specification: `openapi.json` (included in repository for offline development/mocking)

## Notes

* The mailing may contain **invalid e-mail addresses**.
* The API **only accepts authenticated requests via token** (credentials will be provided).
* Token will expires in 30 minutes (need rotation).
* **Details matter**: not everything needs to be fully implemented, but your **decisions and trade-offs will be evaluated and discussed** during review.
* **LLMs/AI could be used** to assist, **as long as you understand and stay in control** of the code and design you submit.

## Expected scope

**Required**

* **Solution architecture**: draw the solution **in terms of components and cloud services** (even if you do not deploy to cloud). Choose whatever artifacts and level of detail you consider essential. Expect this service to scale, handle multiple mailings of different sizes.
* **Implementation** in an **object-oriented language** of your choice.
* **Unit tests** for your API/service.
* **Evidence** of the system running.

**Optional / desirable (include if you feel comfortable or wish to)**

* **Requirements understanding & work organization** (how you decomposed the problem, brief plan, etc.).
* **Software architecture**: Choose whatever artifacts and level of detail you consider essential to explain your software architecture (static / dynamic / packages)
* **Local environment setup solution** (any approach you prefer to spin up and run locally).
* **README** (at your discretion).
* **CI/CD** configuration.

## Non-functional requirements

* The API has a **low rate limit** and it must be respected.
* **All emails** from the CSV must be sent.
* **Security** is fundamental.
* **Extensibility (as a design exercise only):** consider how your design *could* support replacing the email-sending API with another provider. This is purely for evaluation — **your code will not be reused in our products**.
* **Maintainability** of the code is important.
* **Failures** must be handled; the system must be **idempotent**.
* Provide **logs** that help locate and understand issues.

## Deliverables

* Repository link containing what you deem necessary to fulfill the challenge.
* Clear instructions to run locally (and to run tests, if applicable).
* **Evidence** of execution (e.g., screenshots, logs, or a brief report).

## Submission & feedback

* Send the repository link by the agreed date.
* We will provide feedback **within 7 days** after submission.
