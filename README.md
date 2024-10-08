# #5 Recipe Sharing Community

### 1\. Project Overview

The **Recipe Sharing Community** is a full-stack web application aimed at bringing together cooking enthusiasts, providing a platform where users can share, discover, and organize recipes. Targeting home cooks, culinary students, and anyone passionate about cooking, the platform allows users to post favorite recipes, contribute interactive ingredient checklists, and share cooking time estimates. The community fosters sharing culinary knowledge, supporting social engagement.

Key features include user registration, recipe submission with detailed ingredient lists, a built-in cooking timer, and social features such as commenting, rating, following users, and upvoting/downvoting posts. Premium features, such as exclusive content access, will be available through a subscription-based model.

## Live URL
 ```url
   https://recipe-sharing-community-server.vercel.app/api
   ```
### 3\. Functional Requirements

#### 3.1 User Authentication & Authorization

*   **User Registration**: Account creation with email, password, and profile details (e.g., username, profile picture).
*   **Login & JWT-based Authentication**: Secure login with JWT tokens to manage user sessions.
*   **Password Recovery**: Password reset functionality via email.
*   **Secure Password Change**: Ability to update the password after login.

#### 3.2 User Profile Management

*   **Profile Customization**: Users can update personal information such as name, profile picture, and bio.
*   **Social Connectivity**: Users can follow/unfollow others, with follower/following counts displayed.
*   **Premium Membership Subscription**: Users can purchase premium memberships through online payment (AAMARPAY/Stripe). Membership is valid for a specific period and unlocks premium content.

#### 3.3 Recipe Management

*   **My Recipes**: A section displaying the user’s submitted recipes with filtering, searching, pagination, and sorting (user assess).
*   **Recipe Sharing (Creation and Update)**: Rich Text Editor support for formatting recipes and attaching images for visual appeal.
    *   **Ingredient Checklist (optional)**: Users can interact with the checklist to track gathered ingredients.
         - Each ingredient in a recipe will be listed on the screen.
         - Users can check or uncheck the ingredients they've gathered by interacting with the list (e.g., by clicking checkboxes).
         - Once an ingredient is checked, it visually indicates that it's ready, helping users focus on the remaining ingredients.
         - Consider allowing users to also add custom ingredients or remove ones they don’t need.
         - You can enhance this by showing the number of remaining ingredients, or even group them based on type (e.g., spices, vegetables).
    *   **Timer Functionality (optional)**: A built-in timer for tracking cooking durations.
         - Users can start a timer for specific cooking durations (e.g., “Boil for 5 minutes”).
         - The timer counts down and gives a notification (like a sound or popup) when time is up.
         - You can let users set custom durations for each step or even multiple timers for different steps of the recipe running simultaneously.
         - Optionally, allow the timer to pause or reset if needed.
*   **Recipe Deletion**: Users can delete their recipes, and admins can publish/unpublish or delete user-posted recipes.

#### 3.4 Rating, Commenting & Upvote/Downvote System

*   **Rate Recipes**: Users can rate recipes (e.g., 1 to 5 stars). Average ratings will be displayed on the recipe card.
*   **Commenting**: Users can leave comments and have the ability to edit or delete their own comments.
*   **Upvote & Downvote System**: Users can upvote or downvote recipes. Sorting options will display the most upvoted recipes at the top.

#### 3.5 Recipe Feed

*   **Recipe Display**: A dynamic feed displaying recipes with basic information (e.g., title, image, rating). Free content is available to all users, while premium users have access to both free and exclusive content.
*   **Advanced Search & Filter**: Users can search recipes by keywords, ingredients, cooking time, tags (e.g., "vegetarian", "gluten-free").
*   **Infinite Scroll**: Implement infinite scroll for seamless browsing.

#### 3.6 User Management

*   **Admin Controls**: Admins can block/unblock users, delete accounts, and manage recipes and can create, update, delete, and manage admin accounts.

* * *



## Technologies Used
- TypeScript
- Node.js
- Express.js
- MongoDB with Mongoose

# Getting Started

## Prerequisites

* **Software:**
    * Node.js (version 20.11.1 or higher)
    * npm Package Manager

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/Programmer-Manik/RecipeSharingCommunity_Server.git
   ```

