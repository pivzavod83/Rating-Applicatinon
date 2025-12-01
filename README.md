# Rate App

A personal rating application where users can track, organize, and share ratings for anything: movies, restaurants, drinks, experiences, products, and more.  
The system is built around profiles, folders, and items, with optional social features and future expansions planned.

---

## Features

### Profile System
Each user has a customizable profile:
- Profile picture and username  
- Public and private folders  
- Adjustable rating system (e.g. out of 5, out of 10, decimals)  
- Followers and followed profiles  
- Secure login (email + password) stored in a database  
- Each profile represented as a `Profile` class object  

---

## Data Structure Overview

### Profile Class
Represents a single user.

**Features include:**  
- Profile picture  
- Username  
- Public and private folders  
- Preferred rating system  
- Followers and following lists  
- Access to user’s folders and items  

---

### Item Class
Represents a single rated item.

**Private attributes:**  
- `id` (hashed string or int)  
- `folder` (ID reference to parent folder)  
- `name`  
- `rate`  
- `date` (auto-generated)  
- `comment` (optional)  
- `image` (optional)  
- `location` (optional object)

**Public:**  
- Setters and getters  

---

### Folder Class
A folder stores a collection of items.

**Private attributes:**  
- `id` (hashed string or int)  
- `private/public` flag  
- `name`  
- Rating system (object describing scale and rules)  
- List of `Item` objects  

**Public:**  
- Setters and getters  

---

## Planned Features

- **Rating filter/game**  
  Let two users rate each other’s items on a shared scale and compare results.

- **Shared folders**  
  Collaborative folders for two or more users to rate experiences together.

- **Multi-rating shared items**  
  A single item containing ratings from several people.

- **“Choose” feature**  
  Finds the highest-rated item shared by two users and recommends it.

- **Template folders**  
  Pre-made folders for common categories (restaurants, movies, drinks, etc.).

- **Database item lookup**  
  Suggest existing items when adding a new one (reuse photos, locations, etc.).

- **Friend lookup**  
  Quickly check if a friend has rated a certain item.

- **Gift suggestion assistant**  
  AI-driven gift ideas based on a friend’s highly-rated items and interests.

- **“Want to Try” folder**  
  A default folder for things the user wants to check out.

- **Search bar with global averages**  
  Search an item and view average ratings across all users, plus friend-specific ratings.

---

## License
This project is licensed under the **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0)**.  
*Users may view and use the project but may not modify or redistribute derivative versions.*
