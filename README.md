# Solutions

## QA

| Task                           | Estimated Time                 | Solution                                                                                                                                                                                                                                 | Project |
| ----                           | --------------                 | --------                                                                                                                                                                                                                                 | ------- |
| Expand textarea as user types  | 20-40 min depending on context | const textarea = document.getElementById(id);  const heightLimit = //choose height limit; textarea.style.height = '' //reset height; const height = Math.min(textarea.scrollHeight, heightLimit); textarea.style.height = height + 'px'; | CliqUps |
| Set app height based on device | 10-20 min                      | Use window.innerHeight to set the height of a body element. window.screen.height returns a larger screen then the browser's                                                                                                              | Cliqups |
| Speed up image upload          | 4-5 hours depending on context | Use either FileReader/base64 or URL.createObjectURL to create preview images while the actual image uploads. Once loaded, render actual image over the temporary backgroind image. Watch out for orientation on iphone (exif)            | Hoopla  |

## Meteor/React

| Issue                          | Solution                                                                                                                                                                                                                                 | Project |
| ----                           |  --------                                                                                                                                                                                                                                | ------- |
| Cannot find module on import   | Meteor beta expects relative import paths ( from './components/App' )                                                                                                                                                                    | Babel |
