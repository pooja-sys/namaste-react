JavaScript in the Browser vs. React Browsers understand JavaScript and can manipulate the DOM using methods like innerHTML.
React does not directly manipulate the DOM; instead, it uses a Virtual DOM for better performance.
CDN (Content Delivery Network) & Cross-Origin
A CDN hosts JavaScript libraries and allows faster loading of resources.
Cross-Origin issues arise when making requests between different domains, and solutions include CORS policies.
Bundlers (Webpack, Parcel)
Bundlers package and optimize code for production.
create-react-app uses Webpack as its default bundler.
Types of Dependencies
Dev Dependencies (-D) → Needed only during development.
Normal Dependencies → Required for production.
package.json vs. package-lock.json
package.json
Manages project dependencies.
Uses ^ (caret) for minor upgrades and ~ for patch upgrades.
package-lock.json
Locks exact dependency versions.
Ensures consistent installations across different environments.
Tracks transitive dependencies (dependencies of dependencies).
Parcel (Bundler) Features
Dev Build & Local Server
HMR (Hot Module Replacement) → Updates changes without refreshing the page.
File Watching Algorithm → Written in C++ for efficiency.
Caching → Speeds up builds.
Optimizations:
Image optimization
Minification
Bundling & Compression
Consistent Hashing
Code Splitting
Differential Bundling (different bundles for modern & older browsers)
Tree Shaking (removes unused code)
Separate Dev & Prod Bundles
Diagnostics & Error Handling
HTTPS Support
Parcel Commands
Install Parcel:
bash
Copy
Edit
npm install -D parcel
Start Dev Server:
bash
Copy
Edit
npx parcel index.html
Create a Production Build:
bash
Copy
Edit
npx parcel build index.html
Additional Setup
Initialize npm → npm init
Optimize browser support in package.json → Add "browserslist" for better optimizations.pacakage.json add browserlist 
create the package.json inside add start : parcel index.html run code in development mode
build: parcel build index.htm
react is an element and object when render on to the dom is html
jsx is not html
jsx is html like syntax
