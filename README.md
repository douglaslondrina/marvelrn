# Marvel-RN
Small App for a challenge that uses Marvel API to show its heroes.

## Running
```bash
yarn
cd ios; pod install
react-native run-ios
react-native run-android
```

## Screenshots

### iOS
<img src="https://user-images.githubusercontent.com/129619/66735003-89916880-ee3b-11e9-8914-0ea5c7358378.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/129619/66734998-88f8d200-ee3b-11e9-8fad-a17dd01ebf2c.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/129619/66735004-89916880-ee3b-11e9-8f41-f136267de150.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/129619/66735006-89916880-ee3b-11e9-8969-a8c954153bd9.png" width="45%"></img> 

### Android
<img src="https://user-images.githubusercontent.com/129619/66737551-b137ff00-ee42-11e9-8712-2782c790df04.png" width="45%"></img> 
<img src="https://user-images.githubusercontent.com/129619/66735011-8d24ef80-ee3b-11e9-95a7-1a3b7278ba71.png" width="45%"></img>

## Scenarios
  
1. List characters API limited to 5 items each page
   * I decided to fetch 5 instead of the requested 4 itens to improve visually the UI.
2. Filter characters by name
3. Show pagination as per number of characters available
4. Show hero detail in new page

## Behaviours to test

### Main page (if time allows, I will add Unit tests to assert these):
* Main page should render "no itens" child
* Main page should have rendered at least 1 item child if api returns something
* Shanging pages should change the set of itens listed

### Detail page
* Should render character details and image

## Snapshot Tests
* Should render Main page as intended or show connection error
* Should render Detail page as intended or show connection error

## What could be improved
- [ ] Add more visual resources, like icons
- [ ] Add Unit tests, generic snapshots only help when code is production ready and needs to keep visual consistency
- [ ] Fetch more info about characters and redirects
