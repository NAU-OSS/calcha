# Contributing to Calcha
## How to Contribute (issues, pull requests, feature request, etc.)
### Issues
If you encounter an issue when using Calcha, please check the issue tracker before creating a new issue. This way we can be sure the issue is not solved or currently being worked on. Otherwise, please create a new issue!

When creating a new issue, please provide sample code from which the issue can be recreated; please also provide the commands you ran upto and including the (potentially) problematic command; please make sure to provide any error information you received when the issue occured.

### Pull Requests
When submitting code for review, please provide a short description of the changes you made and mention any issues in the tracker you are attempting to fix or implement.

### Feature Requests
To request a new feature, please use the issue tracker and mark your issue with the 'new feature' label. Please provide a short description of what the feature is and does. Discussion and decisions will be made vis-a-vis the comments and subsequent pull requests.

Please make sure to look in the issue tracker to make sure your feature has not been suggested before! In the case that your feature has been suggest, go ahead and give a reaction to show your support! However, because some people may have a similar, but not completely different feature suggestion than yours, feel free to add a comment about what could also be added to facilitate your work!


## Code Style or Formatting Guidelines
When extending the capability of the compiler, you will be writing Hare. Please refer to the style guide for the Hare Programming Lange [here](https://harelang.org/documentation/usage/style.html) for more information on code style.


## Testing Requirements
Testing requirements are enforced through GitHub Actions. If you are making a pull request which deals with an existing piece of the codebase, it is very likely your changes will be tested when pushed. However, if you are adding a new feature, then creating an action to test your code will be discussed and iterated upon as discussion progresses. This is because of the uniqueness of the problems we are trying to solve within this community. Please feel free to submit your own tests before code review to facilitate understanding and discussion of the feature.


## Documentation Standards
It is expected that documentation is updated when fixes are issued. This means return values, edge-cases, errors, etc. are documented in documentation for a specific function.

In the case of adding new features, the documentation will be updated with information about the functions and constructs needed to support the new feature.

Calcha has strongly defined error infrastructure to support readably verbose errors and documentation when things go wrong. Therefore, please extend the existing infrastructure first. If new infrastructure is needed, this will be defined and hashed out in the comments of the respective pull request to ensure the new infrastructure **must** be defined, and to determine it will not interfere with the existing infrastructure.

In the case new infrastructure **must** be defined, then a separate issue and pull request will be started to specifically deligate resources toward developing and documenting the infrastructure. This way, conversations do not become mixed into a single, long conversation thread. The infrastructure to support a new feature (if it is determined is needed) **will be committed first**, and then the new feature will follow.


## Bug Reporting
If you encounter a bug while using Calcha, please check the issue tracker to make sure others have not encountered the same bug. If there is not other report, then please create a new issue following the guidelines stated above. Please mark your issue with the 'bug' label.
