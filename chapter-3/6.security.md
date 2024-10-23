# Security Essentials - Cookies and Privacy
Data breaches and hacks are common, costing companies millions. Many of these breaches are caused by human errors, like **clicking on suspicious emails** or entering passwords into **fake login** pages.

### Cookies
- **Cookies** are small pieces of text used by websites to track your activity.
- They help with useful things, like:
  - Keeping track of items in your shopping cart.
  - Keeping you logged in when you return to a website.
  
### How Cookies Work ?
1. When you visit a website, it sends a cookie to your browser along with the webpage.
2. Your browser stores the cookie and sends it back to the website on your next visit.
3. Cookies are only sent to the website that created them (cookies from `example.com` won't be sent to `example.org`).

### Third-Party Cookies
- Some websites embed **third-party scripts**, like ads or analytics (e.g., Google Analytics).
- These scripts can use **third-party cookies** to track you across different websites.
  - For example, if both `example.com` and `example.org` use the same ad service, the service knows you visited both.
  - This allows advertisers to build a profile of your interests and browsing habits.

## Privacy and Security Concerns
- With broad enough reach (e.g., social media buttons), websites can track you across many sites.

## How to Control Cookie Tracking
You can manage your privacy by controlling how cookies are stored and used:

1. **Ignore Tracking**: Some users choose to ignore cookie tracking.
2. **Limit Tracking**:
   - Block third-party cookies or periodically clear cookies from your browser.
     - Set your browser to not track requests.
     - Clear cookies when you close the browser.
### Summary
- **Cookies** track your activity and can be useful but also raise privacy concerns.
- **Third-party cookies** can track you across multiple sites.
- **Managing cookies** can help protect your privacy but may disrupt how some websites work.

# Password Management
### Root Access
- **Root** is the most privileged user in Linux. Hackers often target it.
- Many admins disable direct root access to prevent unauthorized control of the system.

### User Permissions
- Users have different permissions based on group assignments.
  - **Admins** can create/manage users.
  - **Regular users** have limited permissions.
- Services (e.g., databases) have their own login credentials.

### Password Management  
- Admins often use: - **Password managers** to store encrypted login credentials.
  - **Two-factor authentication (2FA)** for extra security, adding a second layer (e.g., a phone code).
