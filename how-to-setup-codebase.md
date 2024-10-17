Seperate server & client components
* all server functions, actions, api calls -> put in @/server
* dont call api in client components, instead call api/data .. in server component -> pass data to client component via props

Organiza folders
* app
  - (feature group 1)
    - page 1
      - _components   
      - page.tsx
  - _components (components that is used for this page only). _ means private folder
  - layout.tsx
  - page.tsx
  - ..
* public
* @classon: virtual alias folder incase you want to copy code from other packages (of classon).
  - components
  - types
  - lib
* src: --> seperate logic folder and app folder so that we can wrap all code in src folder and build a library (npm package) in next.js 
  - server: prisma, actions, functions. Should use "server only" directive in every file.
  - components: only shared client components
    - ui: shadcn default components only, dont put your custom component here.
  - hooks
  - lib
    - utils.ts: shadcn default file only.
  - config: config, constant
  - types
 
 Note:  
  
