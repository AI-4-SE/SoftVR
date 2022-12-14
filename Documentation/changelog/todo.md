# ToDo List

## Major

(**#1**) = important

- [X] Advanced spawner system (register new in editor, use others, ...) *(12.06.2019)*
- [X] Basic **code city** visualization *(28.06.2019)*
- [X] **#2** Minimal cone tree layout *(05.08.2019)*
- [ ] **#1** Improve code city visualization
  - [X] **#1** Textures to show regions and their performance *(04.09.2019)*
  - [ ] **#2** Show edges/relations between buildings (edge bundling)
  - [ ] Interaction
    - [X] **#1** Selecting elements to open files *(09.08.2019)*
    - [X] Info on hover *(04.07.2019)*
    - [X] Lifting (changing position on y-axis) *(27.08.2019)*
    - [X] Rotation (rotate around y-axis) *(28.08.2019)*
    - [ ] **#3** Jump to according position in code when clicked on NFP texture
    - [ ] "Be the data" approach (maybe?)
- [X] Code Window Content Overview
  - [X] Overview of code window content *(12.07.2019)*
  - [X] Overview of code regions *(18.07.2019)*
  - [X] Where and how to show the content overview window? (either this or heightmap) *(30.08.2019)*
- [ ] **#2** Improve when to update specific parts of the code window (e.g. do not update everything if only feature regions changed)
- [ ] External visualization settings (can be used for later loading of workspace)
  - [ ] Setting: What is displayed by the width, length and height of code city elements
  - [ ] Setting: What is displayed by the city element texture
  - [ ] Setting: What is the position & maximum width, length, height of the code city visualization
  - [ ] Setting: Where is the structure graph positioned & how is it rotated + spacing between nodes, ...
  - [ ] Setting: Where is the feature diagram positioned & how is it rotated + spacing between nodes, ...
- [ ] Overview of feature regions (already in code city texture considered?)
- [ ] Add task window from user study to let users load/make notes
- [ ] 2-Controller interaction (make use of second controller in meaningful way)
- [ ] **#3** New UI (more generic and not all windows opened at once)
  - [ ] Radial Menu (at users hand - maybe activated by gesture)
- [ ] **#3** Advanced accessibility and registration of loaders (like done with spawners)
- [ ] Variability Model improvements (non-boolean & mixed constraints)
- [ ] Text input (VR keyboard)
  - [ ] Search for files and highlighting in e.g. graph or code city
- [ ] Configuration of "mappings" while in application
- [ ] **#3** Storing configured workspace from within application
  - [ ] Store opened file positions
  - [ ] Store configuration of visualizations...
- [ ] Entry room on app startup (similar to SteamVR Home)
  - [ ] Advanced loading screen on startup
  - [ ] Loading workspace/settings from within application
  - [ ] Support of different controller types
  - [ ] Configuration of button layout through user
  - [ ] Use Unity's [Script Execution Order](https://docs.unity3d.com/Manual/class-MonoManager.html) feature
- [ ] Support of different HMDs (e.g. Oculus Rift)
- [ ] Multi-user VR experience
  - [ ] Opening & joining sessions from within the application (maybe in entry room)
  - [ ] Show an avatar for each user that only the other person can see

## Minor
- [X] Enable/Disable all visualizations in UI (includes graphs) *(10.07.2019)*
- [X] Improve overview texture generation by NOT pre-calculating line patterns *(17.07.2019)*
- [X] Nodes rotating towards parent node in cone tree layout *(05.08.2019)*
- [X] Generic code for cone tree layout used by software hierarchy visualization and variability model *(05.08.2019)*
  - [X] Cleanup example scenes accordingly after this modification! *(08.08.2019)*
- [X] Apply minimal cone tree layout algorithm to variability model as well *(06.08.2019)*
- [X] Better font for code in code window (e.g. Consolas - type "monospace" font) *(08.08.2019)*
- [X] **#1** Same color coding for cone tree edges and code city *(21.08.2019)*
- [X] **#3** Improved scrolling using a gesture *(16.08.2019)*
- [X] **#3** Scroll wheel texture and rotation *(22.08.2019)*
- [X] **#1** Add raycast to check that code city hover window is not inside building *(22.08.2019)*
- [X] **#1** Update code city texture when user changes NFP relativity and active NFP *(04.09.2019)*
- [X] **#2** Add possibility to enable/disable code/region overview window *(05.09.2019)*
- [X] **#2** Selecting and configuring numerical options (requires UI concerns) *(12.09.2019)*
- [X] Allow teleport when laser pointer is disabled *(19.09.2019)*
- [ ] Upgrade Unity version and project + ensure everything still works fine
- [ ] Use more Unity Events to react on changes to settings
- [ ] For every change in visualizations (like show/hide) all NFP regions are always re-created (this can be improved!)
- [ ] Horizontal scrolling with new scroll-wheel implementation required?
- [ ] ValueMappings: provide some default color methods for usage in mappings (e.g. Fixed-Red, ...)
- [ ] ValueMappingsLoader: refactoring and generalization of setting types
- [ ] \(Sorting files in cone tree layout by their type to get kinda like a pie chart when color is applied\)?
- [ ] Put overview texture generation in a coroutine to minimize performance impact
- [ ] Improve code overview for the case that there are too many lines resulting in less than one pixel on the texture
- [ ] VariabilityModelSpawner: improve option index retrieval in last version (see comments in code)
- [ ] Add possibility to show/hide code or regions or both in overview window?
- [ ] Tilt hover window of directory graph to user
- [ ] Hints on interaction when user selects a tool for the first time
- [ ] Hints on interaction while using the tools
- [ ] Feature graph: enable parent node if child node activated
  - [ ] Automated check/validation of alternate group selection
- [ ] Possibility to zoom on text for better readability
- [ ] Feature regions counter to show amount of "affected" lines
- [ ] Instant snap to start/end of file instead of "endless" scrolling
- [ ] Improve edge rendering to avoid thin edges when they curve
- [ ] Edges with lighting for better depth clues
- [ ] Improve pointing at files far away (e.g. searching inside a radius)
- [ ] Notation hints on feature graph (e.g. on hover)
- [ ] Information about edges (e.g. on hover)
  - [ ] Type and value/weight of edge
  - [ ] Classes/files to connect between
  - [ ] Line numbers (in code) to connect to
- [ ] Improve counting of edges (add numbers or similar to show)
- [ ] Advanced positioning and rotating of code windows (snap to..., rotate with respect to...)
- [ ] Improve how CodeFile instances are retrieved (assigning an ID for every file and using this internally instead of strings)
- [ ] Code cleanup

## Bugs
- [X] NullPointerException when calling "WindowSpawnedCallback" function with no CodeFile *(12.07.2019)*
- [X] Last line number not shown in code file *(12.07.2019)*
- [X] Cone tree leafs sometimes overlapping a bit in software structure *(21.08.2019)*
- [X] **#1** State of nodes of the variability model not always updating properly *(22.08.2019)*
- [X] Changing controller while pointing at folders/files does not change back color of marked folder/file *(22.08.2019)*
- [X] **#1** Fix code city not having pointer collision *(28.08.2019)* (caused by input module having different layer mask)
- [X] **#1** Overview region sometimes shown black (no longer seen since 23.08.2019 - closed)
- [X] Terminal: Variability Model: Validation color not changed if terminal disabled and option state changes *(19.09.2019)*
- [X] Hover windows still showing if laser pointer was disabled *(19.09.2019)*
- [X] Horizontal scrollbar of code window is sometimes not adjusting the content *(19.09.2019)*
- [X] Rare out of bounds exception when generating overview texture (when only a single line in file) *(19.09.2019)*
- [ ] Overview window scroll for code and regions is hacky and sometimes wobbles a bit
- [ ] Laser pointer sometimes not working right after startup (very rare event that occurred during user study)
