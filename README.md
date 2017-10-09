# Immerse

### Immerse is a virtual reality application to aid in exposure therapy.


## Background & Overview

[Exposure therapy][exposure] is a technique in behavior therapy that has existed since the 1950s and is thought to help treat anxiety disorders.  Exposure therapy involves exposing the patient to the source of anxiety or a representation of it without the intention to cause harm.  According to [this study][study], exposure therapy is the most successful known treatment for phobias.  

Virtual Reality technology represents an incredible new tool for exposure therapy.  Through VR, the core principle of causing no harm to the patient is much more easily fulfilled.  Therapists also have more direct control over the intensity and type of anxiety source.  Cost of treatment is greatly reduced since anxiety sources are digital.    

We intend to create an exposure therapy VR app that will immerse our user in four of the most common phobias: Agoraphobia (fear of crowds), Acrophobia (heights), Arachnophobia (spiders), and Aquaphobia (water).

This project involves:

- Collecting pre-existing VR assets. We will not create original assets given our time constraint.
- Building a frontend interface where users can experience our VR scenes and navigate between
them with a browser or VR headset.
- Hosting our assets in a way that allows for a smooth UX.


## Functionality & MVP

- We will gather a complete set of assets (Pano image/video, sound effects, normal video) for each
of the four phobias.
- We will combine those assets into an immersive VR experience for each phobia.
- We will have a user interface that allows users to select a phobia from a main menu to enter that scene.  Once inside the scene, there will be a button for the user to return to main menu.
- Production README

#### Bonus Features

- Intensity: User or doctor can control intensity level of immersion.  This could take the form of louder sound, more renderings of the anxiety source, or more intense interactions with the anxiety source.
- Proprietary Assets: With the correct hardware (360 camera, sound recorder), assets could be even more finely tuned for exposure therapy.
- Animations for scene transitions (fading in, sliding, etc.).
- Compatibility with multiple VR headsets.
- Countdown once a user selects a phobia scene to enter.  


## Design Documents

- [Wireframes][wireframes]
- [Component Hierarchy][hierarchy]


## Technologies & Technical Challenges

#### Backend:

- None at this point, but will be revisited if necessary.  

#### Frontend:

- React
- React-VR

### Assets

[Assets][assets] were collected from various sources:
- Pano Images: [Flickr][flickr]
- 360 Video: [Youtube][youtube]
- Video: [Pixabay][pixabay]
- Sound effects: [Ambient Mixer][ambientmixer], [Soundbible][soundbible], [Zapsplat][zapsplat]

### Hosting
 - App must be bundled for production before deployment using `npm run bundle`. This creates an `index.bundle.js` file and `client.bundle.js` file in a build folder. These two files, along with the index.html and and locally stored static assets need to be uploaded to web host.
 - First attempts at hosting with Heroku have been unsuccessful but it may be possible with some tweaks.
 - Github Pages seems perfectly capable of hosting the site. [Test Host](https://github.com/NEvans85/vr-test-2) However large files (like 360 videos) will likely need to be hosted from another location to comply with GitHub's storage limitations.


## Accomplished over the Weekend

- Each team member read chapters 1-4 of [this][ebook] tutorial, then implemented the app in
chapter 8 to get a sense of the React-VR structure and workflow.
- Full sets of assets (Pano image/video, sound effects, normal video) were collected for four
main phobias (spiders, heights, open water, and crowds).
- Hosted a sample pano image on Github Pages to get a sense of load times.
- Build Wireframes (John)


## Group Members & Work Breakdown

Our group consists of three members: John Lugtu, Nicholas Evans, and Mike Brinkman.

Work separation for each scene will be one person developing assets and the other two working closely to write the code to implement the scene, incorporating assets as they are available. Roles will rotate day by day.

### Day 1
- Name App
- Title Scene (John)
  + Title Layout
    + Title element
- Dashboard Scene (Mike)
  + Dashboard Layout
    + Dashboard buttons element
      + Button element
- Start Building Soundscapes (Nick)

### Day 2
- Index logic for next scene
- Gather assets for crowd scene, including soundscape
- PhobiaScene (Crowds will be first)
  - Update DashboardScene
    + PhobiaLayout
      + PhobiaElement
        + Update button element

### Day 3
- Spider Scene
- Begin Water Scene

### Day 4
- Finish Water
- Heights Scene

### Day 5
- Debug local version
- Prepare for hosting

### Day 6
- Buffer time for unforeseen difficulties
- Add Bonus Features
  1. Improve UX
    + Scene transitions animations
  2. Support for headset
  3. Intensity feature


[hierarchy]: ./docs/hierarchy.md
[wireframes]: ./docs/wireframes.md
[assets]: ./docs/ASSETS.md
[flickr]: https://www.flickr.com/groups/360degrees/
[pixabay]: https://pixabay.com/
[soundbible]: http://soundbible.com/
[zapsplat]: https://www.zapsplat.com/
[youtube]: https://www.youtube.com/
[ambientmixer]: https://www.ambient-mixer.com/
[ebook]: https://medium.com/coding-artist/learn-react-vr-chapter-1-hello-virtual-world-202241c0cb63
[exposure]: https://en.wikipedia.org/wiki/Exposure_therapy
[study]: https://en.wikipedia.org/wiki/Exposure_therapy#cite_note-17
