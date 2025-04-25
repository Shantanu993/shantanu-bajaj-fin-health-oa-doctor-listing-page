# Doctor Listing Page

[![Deployed on Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-black?style=for-the-badge&logo=vercel)](https://vercel.com/shantanu993s-projects/v0-doctor-listing-page-81)

## Deployment

Project is live at:

**[https://shantanu-bajaj-fin-health-doctor-listing.vercel.app/](https://shantanu-bajaj-fin-health-doctor-listing.vercel.app/)**

## Overview

This project is a doctor listing page with various interactive features to filter and search doctors based on their names, consultation types, specialties, and sorting criteria. It implements client-side functionality for all filters and search after the initial API call.

### Features

1. **Autocomplete Header**
   - A search bar that provides top 3 suggestions based on doctor names.
   - Filters the list of doctors by name when a suggestion is clicked or when Enter is pressed.
   - If no matches are found, no suggestions are shown.

2. **Dynamic Filter Panel**
   - **Single Filter (Radio)**: 
     - Options: Video Consult, In Clinic.
     - Only one option can be selected at a time.
   - **Multi Filter (Checkbox)**: 
     - Options: Doctor specialties.
     - Doctors may have multiple specialties.
     - Multiple filters can be applied simultaneously.
   - **Sort Filter**:
     - Sort by fees (ascending).
     - Sort by experience (descending).
   - Filters work in combination, with the first applied filter taking precedence.

3. **Pagination**
   - Pagination of doctor listings, with support for navigating between pages.
   - The current page number is reflected in the URL and is retained when navigating back or refreshing the page.

4. **Client-Side Filtering, Searching, and Sorting**
   - Filters and sorting happen entirely on the client side after the initial API call.
   - The filters are reflected as query parameters in the URL, and they persist when navigating back.

### API Instructions

- **API URL**: [https://srijandubey.github.io/campus-api-mock/SRM-C1-25.json](https://srijandubey.github.io/campus-api-mock/SRM-C1-25.json)
- Call the API to fetch all doctor data.
- All filtering, searching, and sorting are done on the frontend.
- Applied filters are shown as query parameters in the URL.
- Navigating back or refreshing the page retains the filters via the URL.

### Tech Stack

- **Frontend**: React (with Next.js for server-side rendering)
- **State Management**: React hooks (useState, useEffect, useCallback)
- **CSS**: TailwindCSS for styling
- **Pagination**: Implemented with dynamic page changes and URL state

### How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Shantanu993/shantanu-bajaj-fin-health-oa-doctor-listing-page.git
