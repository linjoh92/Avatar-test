<h1>Create Avatar</h1>

<h3>Add file to /src:</h3>

    - AvatarImg
    - App.css (optional)

1. Create constants/avatarFeatures with 5 arrays, one for each feature. Each array includes 5 objects with names and src: require('../AvatarImg/{imagename}').default.
    - browImages (5x Brows - (name + src))
    - hairImages (5x Hair - (name + src))
    - eyesImages (5x Eyes - (name + src))
    - noseImages (5x Nose - (name + src))
    - mouthImages (5x Mouth - (name + src))

<h3>Components</h3>

1. Header
2. AvatarCretor
3. FeatureSection
4. Button
5. Footer



<h3>Test</h3>

**App.js**
- Render components: Header, CreateAvatar, Button and Footer
- Resetbutton - all selected Avatarfeatures, AvatarName and Input resets

**Header **_({ title, avatarNameInput, handleInputChange })_****
- Headertitle
- Input for AvatarName 
- User input AvatarName shows in AvatarCreator and Footer

**AvatarCreator _({ avatarName })_**
- Rendering the Avatar Face: Renders the avatar's face based on the user's selected features for hair, eyes, brows, nose, and mouth.
- Feature Selection: Allows users to choose from various options for Hair, Eyes, Brows, Nose, and Mouth to customize their avatar.
- Managing Selected Features: Tracks and maintains the state of the selected features (e.g., `SelectedHair`, `SelectedEyes`) which dynamically appear on the Avatar's face.

**FeatureSection _({ featureType, images, selectedFeature, handleFeatureClick, "data-testid": testId })_**
- Layout for display the five AvatarFeatcher categorys - FeatureType and data-testid 
- Map the imges:
    * key
    * src
    * className
    * alt-text
    * width
    * onClick (handelFeatureClick(feature))

**Button _({ onClick, CTA })_**
 - Button
 - Prop - CTA 
 - Prop - OnClick

**Footer _({ avatarName })_**
 - Footertext "Copywrite © 2023"
 - Render Avatarname when added input in header
<img width="995" alt="Skärmavbild 2023-11-28 kl  10 18 05" src="https://github.com/linjoh92/Avatar-test/assets/116895401/4541ddb1-de16-44b1-a214-3b836128e3f2">
<img width="986" alt="Skärmavbild 2023-11-28 kl  10 18 22" src="https://github.com/linjoh92/Avatar-test/assets/116895401/815f62ab-fb4c-4fad-9da0-52b8e6719650">
