<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Portal</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Base styles for Inter font and general layout */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f2f5; /* Light gray background */
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh; /* Ensure it takes full viewport height */
            box-sizing: border-box; /* Include padding in element's total width and height */
        }

        /* Main Dashboard Container - visible after login */
        .dashboard-container {
            display: flex;
            background-color: #fff;
            @apply shadow-2xl rounded-xl overflow-hidden;
            max-width: 1400px;
            width: 100%;
            min-height: 800px;
            visibility: hidden; /* Hidden by default, shown by JS on login */
            opacity: 0; /* Fade in */
            transition: visibility 0s, opacity 0.5s ease-in-out;
        }
        .dashboard-container.visible {
            visibility: visible;
            opacity: 1;
        }

        /* Login Container - visible before login */
        .login-container {
            background-color: #fff;
            @apply shadow-2xl rounded-xl p-8 md:p-12 lg:p-16 w-full max-w-md;
            text-align: center;
            visibility: visible; /* Visible by default, hidden by JS on login */
            opacity: 1; /* Fade out */
            transition: visibility 0s, opacity 0.5s ease-in-out;
        }
        .login-container.hidden {
            visibility: hidden;
            opacity: 0;
            position: absolute; /* Prevent taking up space when hidden */
            left: -9999px; /* Move off-screen when hidden */
        }

        /* Login Page Specific Styles (integrated) */
        .login-container .logo {
            font-size: 2.5rem; /* text-5xl */
            font-weight: 800; /* font-extrabold */
            color: #dc2626; /* Red color */
            margin-bottom: 2rem;
            letter-spacing: -0.05em; /* tighter letter spacing */
        }
        .login-container .form-group {
            margin-bottom: 1.5rem;
            text-align: left;
        }
        .login-container .form-group label {
            display: block;
            font-size: 0.95rem; /* text-base */
            font-weight: 600; /* font-semibold */
            color: #4b5563; /* text-gray-600 */
            margin-bottom: 0.5rem;
        }
        .login-container .form-group input {
            width: 100%;
            padding: 0.85rem 1rem; /* Slightly more padding */
            border: 1px solid #d1d5db; /* border-gray-300 */
            border-radius: 0.5rem; /* rounded-lg */
            font-size: 1rem; /* text-base */
            color: #1f2937; /* text-gray-800 */
            background-color: #f9fafb; /* bg-gray-50 */
            transition: border-color 0.2s ease, box-shadow 0.2s ease;
        }
        .login-container .form-group input:focus {
            outline: none;
            border-color: #ef4444; /* red-500 */
            box-shadow: 0 0 0 3px rgba(239, 68, 68, 0.3); /* red-500 with opacity */
        }
        .login-container .login-button {
            width: 100%;
            background-color: #dc2626; /* Red background */
            color: #fff;
            padding: 1rem 1.5rem; /* Larger padding */
            border-radius: 0.75rem; /* rounded-xl */
            font-size: 1.125rem; /* text-lg */
            font-weight: 700; /* font-bold */
            border: none;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.2s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            margin-top: 1.5rem;
        }
        .login-container .login-button:hover {
            background-color: #b91c1c; /* Darker red */
            transform: translateY(-2px);
            box-shadow: 0 6px 8px rgba(0,0,0,0.15);
        }
        .login-container .links-container {
            margin-top: 1.5rem;
            font-size: 0.95rem;
            color: #6b7280; /* text-gray-500 */
        }
        .login-container .links-container a {
            color: #dc2626; /* Red link color */
            text-decoration: none;
            font-weight: 600;
            transition: color 0.2s ease;
        }
        .login-container .links-container a:hover {
            color: #b91c1c; /* Darker red on hover */
            text-decoration: underline;
        }
        .login-container .separator {
            margin: 1.5rem 0;
            position: relative;
            text-align: center;
        }
        .login-container .separator::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 0;
            right: 0;
            border-top: 1px solid #e5e7eb; /* border-gray-200 */
            z-index: 0;
        }
        .login-container .separator span {
            background-color: #fff;
            padding: 0 10px;
            position: relative;
            z-index: 1;
            color: #9ca3af; /* text-gray-400 */
            font-size: 0.875rem;
        }
        .login-container .social-login button {
            width: 100%;
            padding: 0.85rem 1rem;
            border: 1px solid #d1d5db;
            border-radius: 0.5rem;
            font-size: 1rem;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            background-color: #fff;
            color: #374151; /* text-gray-700 */
            cursor: pointer;
            transition: background-color 0.2s ease, border-color 0.2s ease;
            box-shadow: 0 1px 2px rgba(0,0,0,0.05);
        }
        .login-container .social-login button:hover {
            background-color: #f3f4f6; /* bg-gray-100 */
            border-color: #9ca3af;
        }
        .login-container .social-login .icon {
            font-size: 1.25rem;
        }


        /* Sidebar Styling */
        .sidebar {
            width: 280px; /* Fixed width for sidebar */
            background-color: #dc2626; /* Red background */
            color: #fff;
            padding: 32px 0; /* More padding top/bottom */
            display: flex;
            flex-direction: column;
            align-items: center;
            border-top-left-radius: 0.75rem; /* rounded-xl */
            border-bottom-left-radius: 0.75rem; /* rounded-xl */
            flex-shrink: 0; /* Prevent shrinking */
        }
        .user-profile {
            text-align: center;
            margin-bottom: 40px; /* Increased margin */
            padding: 0 20px;
        }
        .profile-pic-container {
            width: 90px; /* Slightly larger image */
            height: 90px;
            border-radius: 50%;
            overflow: hidden;
            border: 3px solid #fff; /* Thicker white border */
            margin: 0 auto 12px;
        }
        .profile-pic {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .user-name {
            font-size: 1.375rem; /* text-2xl */
            font-weight: 700; /* font-bold */
            margin-bottom: 4px;
        }
        .user-faculty {
            font-size: 0.95rem; /* Slightly larger text-sm */
            opacity: 0.9;
        }
        .navigation {
            width: 100%;
            flex-grow: 1;
        }
        .navigation ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        .navigation li {
            width: 100%;
            margin-bottom: 6px; /* Slightly less margin between items */
        }
        .navigation a {
            display: flex;
            align-items: center;
            padding: 14px 28px; /* More padding for links */
            color: #fff;
            text-decoration: none;
            font-size: 1.05rem; /* Slightly smaller text-lg */
            font-weight: 500; /* Medium weight for general links */
            transition: background-color 0.3s ease, padding-left 0.3s ease;
            position: relative;
        }
        .navigation a:hover {
            background-color: rgba(255, 255, 255, 0.15); /* More visible hover */
            padding-left: 32px; /* Slight indent on hover */
        }
        .navigation a.active {
            background-color: #b91c1c; /* Darker red for active state */
            font-weight: 600; /* Semibold for active link */
        }
        .navigation a.active::before {
            content: '';
            position: absolute;
            left: 0;
            top: 0;
            bottom: 0;
            width: 6px;
            background-color: #facc15; /* Yellow indicator */
            border-top-right-radius: 9999px;
            border-bottom-right-radius: 9999px;
        }
        .navigation .icon {
            margin-right: 16px; /* More space for icon */
            font-size: 1.35rem; /* Larger icon */
            width: 24px; /* Fixed width to align icons */
            text-align: center;
        }
        /* Removed Feedback Button CSS as the button itself is removed */


        /* Main Content Area */
        .main-content {
            flex-grow: 1;
            background-color: #fff;
            padding: 40px; /* More padding for content */
            border-top-right-radius: 0.75rem; /* rounded-xl */
            border-bottom-right-radius: 0.75rem; /* rounded-xl */
            display: flex;
            flex-direction: column;
        }
        .main-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 32px; /* Increased margin */
            border-bottom: 1px solid #e5e7eb; /* border-gray-200 */
            padding-bottom: 20px; /* More padding below line */
        }
        .main-header h2 {
            font-size: 2rem; /* text-4xl */
            font-weight: 800; /* Extra bold */
            color: #1f2937; /* text-gray-800 */
        }
        .header-controls {
            display: flex;
            gap: 16px; /* More space between controls */
            align-items: center;
        }
        /* Removed select dropdowns CSS as they are removed */
        .header-controls .red-button {
            background-color: #dc2626; /* Red */
            color: #fff;
            padding: 10px 16px; /* More padding */
            border-radius: 0.5rem; /* rounded-lg */
            font-size: 1.35rem; /* Larger icon */
            display: flex;
            align-items: center;
            justify-content: center;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.2s ease;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .header-controls .red-button:hover {
            background-color: #b91c1c; /* Darker red */
            transform: translateY(-1px);
        }

        /* Dashboard Grid Layout */
        .dashboard-grid {
            display: grid;
            grid-template-columns: 2fr 1fr; /* Two columns, left wider than right */
            gap: 32px; /* Increased gap */
            flex-grow: 1; /* Allow grid to take available space */
        }
        .left-column, .right-column {
            display: flex;
            flex-direction: column;
            gap: 32px; /* Increased gap */
        }

        /* Noticeboard List */
        .noticeboard-list {
            background-color: #fff;
            border-radius: 0.75rem; /* rounded-xl */
            overflow: hidden;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05); /* Light shadow */
        }
        .notice-item {
            display: flex;
            align-items: flex-start; /* Align icon to top of text */
            padding: 20px 24px; /* More padding */
            border-bottom: 1px solid #e5e7eb; /* border-gray-200 */
            gap: 20px; /* More space */
        }
        .notice-item:last-child {
            border-bottom: none;
        }
        .notice-icon {
            font-size: 2.25rem; /* Larger icon */
            color: #dc2626; /* Red icon */
            width: 56px; /* Fixed size */
            height: 56px;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: #fee2e2; /* Red-100 */
            border-radius: 0.75rem; /* rounded-lg */
            flex-shrink: 0;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1); /* Subtle shadow */
        }
        .notice-text {
            flex-grow: 1;
        }
        .notice-date {
            font-size: 0.8rem; /* Slightly larger text-xs */
            color: #6b7280; /* text-gray-500 */
            margin-bottom: 6px;
            font-weight: 500;
        }
        .notice-title {
            font-size: 1.25rem; /* text-xl */
            font-weight: 700; /* font-bold */
            color: #1f2937; /* text-gray-800 */
            margin-bottom: 8px;
            line-height: 1.3;
        }
        .notice-excerpt {
            font-size: 0.95rem; /* Slightly larger text-sm */
            color: #6b7280; /* text-gray-500 */
            line-height: 1.5;
        }
        .notice-button {
            background-color: transparent;
            color: #dc2626; /* Red text */
            border: 2px solid #dc2626; /* Thicker red border */
            padding: 10px 20px;
            border-radius: 9999px; /* rounded-full */
            font-size: 0.95rem; /* Slightly larger text-sm */
            font-weight: 600; /* font-semibold */
            cursor: pointer;
            transition: all 0.3s ease;
            flex-shrink: 0;
            min-width: 120px; /* Ensure button has some minimum width */
            text-align: center;
        }
        .notice-button:hover {
            background-color: #dc2626;
            color: #fff;
            transform: translateY(-1px);
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .view-more-notices {
            background-color: #fff;
            color: #dc2626; /* Red text */
            border: 2px solid #dc2626; /* Red border */
            padding: 12px 24px;
            border-radius: 0.75rem; /* rounded-xl */
            font-weight: 700; /* font-bold */
            cursor: pointer;
            width: 100%;
            text-align: center;
            transition: all 0.3s ease;
            margin-top: 24px; /* Space from notice list */
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }
        .view-more-notices:hover {
            background-color: #dc2626;
            color: #fff;
            transform: translateY(-2px);
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        /* Bottom Widgets */
        .bottom-widgets {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 24px;
        }
        .widget {
            background-color: #fff;
            padding: 24px; /* More padding */
            border-radius: 0.75rem; /* rounded-xl */
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
            text-align: center;
            display: flex; /* Use flex for internal alignment */
            flex-direction: column;
            justify-content: space-between; /* Push content apart */
        }
        .widget h3 {
            font-size: 1.375rem; /* text-2xl */
            font-weight: 700; /* font-bold */
            color: #1f2937; /* text-gray-800 */
            margin-bottom: 16px; /* Increased margin */
        }
        .current-enrolment p {
            font-size: 1.15rem; /* Slightly larger text-lg */
            color: #4b5563; /* text-gray-600 */
            margin-bottom: 20px; /* Increased margin */
            flex-grow: 1; /* Push button to bottom */
        }
        .current-enrolment button {
            background-color: #dc2626; /* Red */
            color: #fff;
            padding: 10px 20px;
            border-radius: 9999px; /* rounded-full */
            font-weight: 600; /* font-semibold */
            border: none;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.2s ease;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .current-enrolment button:hover {
            background-color: #b91c1c; /* Darker red */
            transform: translateY(-1px);
        }

        .assessment-status {
            text-align: left; /* Align assessment status text left */
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .assessment-status h3 {
            text-align: center; /* Center heading */
        }
        .assessment-status .status-bar-wrapper {
            position: relative;
            margin-bottom: 16px;
            flex-grow: 1;
            display: flex;
            align-items: center; /* Center vertically */
            padding-bottom: 12px; /* Space for percentage */
        }
        .assessment-status .status-bar {
            width: 100%;
            background-color: #e5e7eb; /* bg-gray-200 */
            height: 14px; /* Thicker bar */
            border-radius: 9999px; /* rounded-full */
            overflow: hidden;
        }
        .assessment-status .progress {
            background-color: #22c55e; /* Green-500 */
            height: 100%;
            border-radius: 9999px;
            transition: width 0.5s ease-in-out; /* Smooth transition */
        }
        .assessment-status .percentage {
            position: absolute;
            right: 0; /* Align to the right edge of the bar */
            top: 50%;
            transform: translateY(-50%) translateX(calc(100% - 70%)); /* Adjust based on progress to show near end */
            font-size: 0.9rem; /* text-sm */
            font-weight: 700; /* Bold */
            color: #1f2937; /* text-gray-800 */
            background-color: #dcfce7; /* Green-100 */
            padding: 2px 8px;
            border-radius: 9999px;
            box-shadow: 0 1px 2px rgba(0,0,0,0.1);
        }
        .assessment-status .status-text {
            font-size: 1.05rem; /* Slightly larger text-base */
            color: #4b5563; /* text-gray-600 */
            text-align: center;
            font-weight: 500;
        }

        /* Upcoming Activity */
        .upcoming-activity {
            background-color: #fff;
            padding: 24px;
            border-radius: 0.75rem; /* rounded-xl */
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
            flex-grow: 1; /* Allow to fill space */
            display: flex;
            flex-direction: column;
        }
        .upcoming-activity h3 {
            font-size: 1.375rem; /* text-2xl */
            font-weight: 700; /* font-bold */
            color: #1f2937; /* text-gray-800 */
            margin-bottom: 20px;
        }
        .upcoming-activity ul {
            list-style: none;
            padding: 0;
            margin: 0;
            flex-grow: 1; /* Allows list to expand */
        }
        .upcoming-activity li {
            display: flex;
            align-items: flex-start;
            gap: 16px; /* More space */
            margin-bottom: 20px; /* More margin */
        }
        .activity-bullet {
            width: 12px; /* Slightly larger bullet */
            height: 12px;
            border-radius: 50%;
            flex-shrink: 0;
            margin-top: 6px; /* Align with text */
            box-shadow: 0 1px 2px rgba(0,0,0,0.1);
        }
        .red-bullet { background-color: #dc2626; } /* Red */
        .blue-bulle
