## DevNet Create 2021 - LT06: Building Stability, Performance &amp; Scale into SecureX Orchestration Workflows

[About DevNet Create 2021](https://developer.cisco.com/devnetcreate/2021) | [**Link to Session Presentation**]()

There are **three** branches in this repository:

1. `main`: This is the default branch. If you're reading this, you're in the `main` branch. Workflows used to demonstrate concepts in the lightning talk are available here:
    1. [Hello DevNet Create!](): A simple workflow to make an API Request to jsonplaceholder.typicode.com, parse the response & set an output variable with the parsed response
    2. **Breadcrumbs (Logging & Tracing Framework)**

        > For original code & documentation, please visit [ciscomanagedservices/sxo-utilities](https://github.com/ciscomanagedservices/sxo-utilities) & review the section on "Breadcrumbs"
        1. [(Logging) Hello DevNet Create!](): Added Breadcrumbs Logging Blocks after each activity to capture progress of the preceeding activity. Also added `/garbage` to the 'Relative URL' of the web service request activity to introduce an intential failure that's captured by Breadcrumbs.
        2. [(Tracing) Hello DevNet Create!](): A simple workflow to read from the `All My Breadcrumbs` table and provide a JSON response with the stack trace captured above.
    3. **Oversight (Error Handling & Alerting Framework)**

        > For original code & documentation, please visit [ciscomanagedservices/sxo-utilities](https://github.com/ciscomanagedservices/sxo-utilities) & review the section on "Oversight"
        1. [(With Error) Hello DevNet Create!](): Added `/garbage` to the 'Relative URL' of the web service request activity to introduce an intential failure
        2. [(Error Handler) Hello DevNet Create!](): A simple workflow to notify via a text to a Webex space when an error occurs
    4. [Import from GitHub](): A workflow that triggers off notifications of new commits to the `prod` branch and pulls down the committed workflow into the Org. 

        > Please note that this workflow is intentionally limited for demonstration purposes only & may not import all workflow dependencies. 'Watch' the [ciscomanagedservices/sxo-utilities](https://github.com/ciscomanagedservices/sxo-utilities) repository to be notified when this workflow supports additional capabilities.
2. `dev`: This branch contains the Dev workflow (a copy of the "[Hello DevNet Create!]()" workflow) & GitHub Actions ([AutoDoc](https://github.com/ciscomanagedservices/sxo-autodoc) & [Analyzer](https://github.com/ciscomanagedservices/sxo-analyzer)) used to demonstrate Continuous Integration & Deployment (CI/CD).
3. `prod`: This branch contains the Prod workflow (pushed from the `dev` branch) & a GitHub Action to dispatch an email on commit to a mailbox that [this import workflow]() on our Production Org monitors. This is the branch our Production Org pulls from.

Please note that workflow content & GitHub Actions in this repository will not be kept up to date with new code releases/patches. Please refer to the original repositories (linked above where applicable) for updates. If you're a DevNet Create 2021 attendee, you may create an issue on this repository or reach out to us via email for queries and/or feedback.

Oh and, while you're here, you may want to check out [some of our other content](https://github.com/ciscomanagedservices) as well 🚀 

---

Contributors:

1. Aman Sardana (amasarda@cisco.com)
2. Anant Nambiar (ananambi@cisco.com)

Cisco CX Managed Services - Operate, September 2021
