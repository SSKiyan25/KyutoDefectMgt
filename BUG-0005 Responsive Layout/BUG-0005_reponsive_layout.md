# STORE-0004: UI - Map Component Not Mobile-Friendly

[Summary]
The main map component of the ViSiTa application is not responsive and does not display properly on mobile devices. The map fails to adapt to smaller screen sizes, resulting in poor usability, difficulty accessing store icons, and parts of the map being cut off or inaccessible on mobile devices.

[Precondition]

- Software version: ViSiTa (HG.011.000)
- Software configuration: Default UI settings
- Hardware specifications: Various mobile devices (smartphones and tablets)
- Network configuration: Standard internet connection

[Steps to reproduce]

1. Access the ViSiTa application from a mobile device (smartphone or tablet)
2. Log into the application
3. Navigate to the main page with the map interface
4. Observe how the map component displays on the mobile screen
5. Attempt to interact with store icons on the map
6. Try to zoom, pan, or navigate the map on the mobile device

[Actual results]

- The map component does not resize appropriately for mobile screens
- Store icons may be difficult to tap accurately due to sizing issues
- Parts of the map may be cut off or require excessive scrolling to access
- Map controls (zoom, pan) are not optimized for touch interaction
- Overall poor user experience on mobile devices when interacting with the map

[Expected results]

- The map component should be fully responsive and adapt to all screen sizes
- Map should automatically resize to fit mobile screens without requiring horizontal scrolling
- Store icons should be appropriately sized for easy tapping on touch screens
- Map controls should be optimized for touch interaction
- Full functionality of the map should be preserved across all devices

[Additional information]
As shown in the included screenshot, the map component takes up excessive space and doesn't adapt properly to mobile screens. Users on mobile devices have difficulty interacting with this critical component of the application, significantly hampering the mobile user experience.

[Is this Breakage?]
Yes, severe mobile usability issue

[Severity: How does this problem impact the customer/user?] 8. Major functionality inaccessible on mobile devices

[Likelihood: How often will a customer/user use this feature/function?] 9. Extremely high, main component of the application

[Repeatability: Is this problem easily reproducible?] 10. 100% Reproducible on all mobile devices

[Impacted Test Cases]
STORE-0004

[Impact Sizing (in days)]
2-3 days
