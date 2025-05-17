# AUTH-0007: Authentication - Password Reset Timing Issue

[Summary]
When users make multiple password reset requests in succession, the system incorrectly reports that the email doesn't exist instead of indicating that a previous request is still being processed. The system also lacks appropriate feedback about the waiting period between requests.

[Precondition]

- Software version: ViSiTa (HG.011.000)
- Software configuration: Default authentication settings
- Hardware specifications: N/A (server-side issue)
- Network configuration: Standard internet connection

[Steps to reproduce]

1. Navigate to the login page
2. Click on "Forgot Password" link
3. Enter a valid registered email and submit the request
4. Immediately attempt to submit another password reset request for the same email
5. Observe the error message received

[Actual results]

- The system responds with "Email not found" or similar error message when making multiple requests
- No indication is given that a previous request is still being processed
- No information provided about required waiting time between requests
- Users may interpret the error as their email not being registered in the system

[Expected results]

- The system should inform the user that a previous request is still being processed
- Clear indication of waiting period between password reset requests (e.g., "Please wait 10 minutes before requesting another reset")
- Status indicators showing that the request is being processed
- Consistent messaging that doesn't falsely indicate the email doesn't exist

[Additional information]
Takes too much time to receive request, does not indicate to wait if multiple requests to reset password as well. Instead of saying "wait", it will say email not exists. Overall, it lacks information that the user should be aware upon requesting and to avoid spamming.

[Is this Breakage?]
No, improvement to existing implementation

[Severity: How does this problem impact the customer/user?] 7. Critical user experience and security issue

[Likelihood: How often will a customer/user use this feature/function?] 4. Medium, affects users who forget passwords or need to reset them

[Repeatability: Is this problem easily reproducible?] 10. 100% Reproducible

[Impacted Test Cases]
AUTH-0007

[Impact Sizing (in days)]
Less than a day
