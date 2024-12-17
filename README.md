This is a Google Apps Script that creates a conference room schedule viewer that is deploye through the web app. Here are the step-by-step instructions to implement this script:

1. **Create a New Google Apps Script Project**
   - Go to script.google.com
   - Click "New Project"
   - Give your project a meaningful name (e.g., "Conference Room Schedule")

2. **Get Your Calendar ID**
   - Open Google Calendar
   - Go to your conference room calendar settings
   - Scroll down to "Integrate calendar"
   - Copy the Calendar ID (it will look like: example@group.calendar.google.com)
   - Replace 'ENTER_CALENDAR_ID_HERE' in both functions with your copied Calendar ID

3. **Add Background Image (Optional)**
   - Upload your desired background image to Google Drive
   - Make the image publicly accessible by right-clicking → Share → Anyone with the link
   - Get the image URL by right-clicking → Get link
   - Replace 'ENTER_IMG_URL_HERE' with your image URL
   - If you don't want a background image, you can remove the entire `body::after` CSS block

4. **Deploy the Web App**
   - Click on "Deploy" → "New deployment"
   - Click "Select type" → "Web app"
   - Fill in the following:
     - Description: Conference Room Schedule
     - Execute as: Me
     - Who has access: Choose appropriate access level (Anyone, Anyone within your organization, or Specific users)
   - Click "Deploy"
   - Authorize the app when prompted
   - Copy the deployment URL provided

5. **Testing the Web App**
   - Open the deployment URL in a new tab
   - The page should display today's events for your conference room
   - The display will automatically refresh every 60 seconds
   - Events will be marked as either "In Progress" or "Upcoming"

6. **Troubleshooting**
   - If no events appear, verify:
     - The Calendar ID is correct
     - There are events scheduled for today
     - You have permission to access the calendar
   - If the background image doesn't appear:
     - Check if the image URL is accessible
     - Verify the image URL is correctly formatted

The web app will show a table with three columns:
- Time (showing start and end times)
- Event (showing the event title)
- Status (showing if the event is "In Progress" or "Upcoming")

The page uses a clean, professional design with:
- Blue headers (#2885C3)
- Alternating row colors for better readability
- Hover effects on table rows
- Responsive layout that centers content
- Arial font for clean typography

Would you like me to explain any particular part of the setup process in more detail?
