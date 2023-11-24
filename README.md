**Create Avatar**

Add file to /src:
- AvatarImg
- App.css (optional)

1. Create constants/avatarFeatures with 5 arrays, one for each feature. Each array includes 5 objects with names and src: require('../AvatarImg/{imagename}').default.
    - browImages (5x Brows - (name + src))
    - hairImages (5x Hair - (name + src))
    - eyesImages (5x Eyes - (name + src))
    - noseImages (5x Nose - (name + src))
    - mouthImages (5x Mouth - (name + src))

**_Components_**

1. Header
2. AvatarCretor
3. FeatureSection
4. Button
5. Footer

**_Test_**

App.js
- Render components: Header, CreateAvatar, Button and Footer
- Resetbutton - all selected Avatarfeatures, AvatarName and Input resets

Header **_({ title, avatarNameInput, handleInputChange })_**
- Headertitle
- Input for AvatarName 
- User input AvatarName shows in AvatarCreator and Footer

AvatarCreator **({ avatarName })**
- Rendering the Avatar Face: Renders the avatar's face based on the user's selected features for hair, eyes, brows, nose, and mouth.
- Feature Selection: Allows users to choose from various options for Hair, Eyes, Brows, Nose, and Mouth to customize their avatar.
- Managing Selected Features: Tracks and maintains the state of the selected features (e.g., `SelectedHair`, `SelectedEyes`) which dynamically appear on the Avatar's face.

FeatureSection **({ featureType, images, selectedFeature, handleFeatureClick, altTextModifier = 1, width = 100 , "data-testid": testId })** 
- Layout for display the five AvatarFeatcher categorys - FeatureType and data-testid 
- Map the imges:
    * key
    * src
    * className
    * alt-text
    * width
    * onClick (handelFeatureClick(feature))

Button **({ onClick, CTA })**
 - Button
 - Prop - CTA 
 - Prop - OnClick

Footer **({ avatarName })**
 - Footertext "Copywrite © 2023"
 - Render Avatarname when added input in header
