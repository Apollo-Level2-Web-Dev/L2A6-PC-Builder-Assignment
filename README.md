# Assignment 6: Simple PC Builder Website using Next.Js (Frontend Category)

### Main Part:

Requirements:

Build a clean and straightforward PC Builder website for PC parts and components using Next.js. The website should include a PC Builder tool where users can add selected PC components to build their own PC.

### Navbar:

- Add a button named **PC Builder**.
- Clicking on the **PC Builder** button should redirect the user to the PC Builder page to start building their PC.
- The navbar should also have a Categories dropdown with the following categories:
    - CPU / Processor
    - Motherboard
    - RAM
    - Power Supply Unit
    - Storage Device
    - Monitor
    - Others
    
    Each category should have a corresponding route. (SSG implementation)

### Home Page: (SSG implementation)

- The home page should feature at least 6 random PC components as Featured Products.
    - Each Featured product card should display the following properties:
        - Image
        - Product Name
        - Category
        - Price
        - Status ( In Stock | Out of stock)
        - Rating (Out of 5 Stars)
    - Each featured product will be clickable and should take the user to the product detail page. (Button/Entire Card)

- There should be 6 Featured Categories under the Featured Product section. The Categories are:
    - CPU / Processor
    - Motherboard
    - RAM
    - Power Supply Unit
    - Storage Device
    - Monitor
    - Others (GPU, Mouse, Keyboard, etc…)

### Featured Category Sections: (SSG implementation)

- Each featured category should be clickable.
- Clicking on any of the Featured Categories will redirect the user to another page where at least 3 products of that category will be displayed.
- Each product card on this page should show the following properties:
     - Image
        - Product Name
        - Category
        - Price
        - Status ( In Stock | Out of stock)
        - Rating (Out of 5 Stars)
- Each product retrieved after querying on this page will also be clickable and should take the user to the product detail page.

### Product Detail Page / Route: (SSG implementation)

- Product Details:
    - Each PC Component must have the following properties:
        - Image
        - Product Name
        - Category
        - Status: In Stock | Out of stock
        - Price
        - Description
        - Key Features (like Brand, Model, Specification, Port, Type, Resolution, Voltage, etc)
        - Individual Rating (Out of 5 Stars)
        - Average Rating (Out of 5 Stars)
        - Reviews

### PC Builder Page: (SSR implementation)

- The PC Builder page should have category sections as follows:
    - CPU / Processor
    - Motherboard
    - RAM
    - Power Supply Unit
    - Storage Device
    - Monitor
- Each category will have a **Choose/Select** Button.
- Clicking on the **Choose/Select** Button will take the user to another page where at least 3 components of that specific category will be displayed.
- Each component card on this page should show the following properties:
    - Image
    - Product Name
    - Category
    - Price
    - Status
    - Rating
- Each component card on that page will have an **Add To Builder** Button.
- Clicking on this button will redirect the user to the PC Builder page, and it will update the state of that selected category section in the PC Builder Page with the selected component below. (You can use Redux / Context API to create a central store for this)
- After adding at least 5 - 6 Components (CPU, RAM, Power Supply, Storage, Motherboard, Casing), the user will be able to click on the **Complete Build** button. (This button will be disabled unless the user adds at least 5-6 of the mentioned components)

### Bonus Part:

- The PC Builder Page should be a protected/private route (only logged-in users can visit this route). You have to use NextAuth with at least one social login (Google/Github) provider to enable user authentication.
- Clicking on the **Complete Build** button will show a success alert.
- The Home page should also have a hero section/banner section and a footer.
- The entire application must be responsive for both mobile and desktop devices to ensure an enjoyable user experience across all devices.
- Create a [ReadMe.md](http://ReadMe.md) file describing your application, explaining its features, and providing clear instructions on how to run the project.

# Deadline:
60 Marks ( Till 29 July, Saturday 11.59 PM )
50 Marks ( Till 30 July, Sunday 11.59 PM )


What to submit
Deployed Frontend Live Link ( Vercel or any other platform)
Your Frontend Github Repository Link
You should add the links to the readme.md file.

# Notes

1. To manage the product's data, you need to create your own backend. This backend could be a single-page backend server or integrated with Next API routes.
2. Do not use 'app' router.
