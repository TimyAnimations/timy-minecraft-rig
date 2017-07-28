# timy-minecraft-rig

Timy's Rig v7.0.0
Make sure you Enable Auto Run Python Scripts in the User Preferences!
This rig is bundled into an addon for easy installation and appending

Rig Features:
	
    Compatible with Blender Internal Render and Cycles Render   
    Compatible with 1.7 and 1.8 Skins
    Compatible with Alex or Steve arm model
    Download skin and cape from username
    Optifine/Custom Cape support
    FK and IK controls
    Fancy Feet (Toggable)
    Auto extrusion of 1.8 and hat layers (Toggable)
    Sharp, Smooth, or No Bends for legs and arms (Toggable)
    Different rig styles or shape (Toggable)
    All types of armor and elytra (Toggable)
    Color options for Leather armor
    Glossy material for Iron, Gold, and Diamond armor (Toggable)
    Enchanted effect for all armor (Toggable)
    Facial Features (Toggable)
    
Custom UI settings:
	
    Global UI Panel:
        Notifications of rig information or errors
        Mode Switches
            Animation Mode :: Shows all Bones needed for animation.
            Edit Mode :: Turns on selection of the mesh for custom extrude/editting the meshes, also hides all bones except the Armature Select Bone.
            Preview Mode :: Hides all bones except the Armature Select Bone.    
         
    Animation UI Panel:
        Toggle to show and hide Advanced Controllers
        Fk/Ik Controls:
            IK and FK Switches for Arms and Legs
            Local IK for arms (Shoulders can be rotated like FK while the IK controller also moves the arm)
        
    Edit UI Panel:
        Rig Properties:
            Skin:
                Username (Allows you to type in a Minecraft Username to get their skin)
                Skin Texture (Allows you to change the skin from the UI side panel)  
                Prefer Optifine Capes (Prefer Optifine capes over Minecraft capes when downloading a skin)
                3D Layers (Makes all 1.8 Layers and the Hat Layer extruded)
            Material:
                Subsurface Scattering (Use Subsurface Scattering, looks good but takes longer to render)
            Style:
                Default, Curvy, Lemon, Chubby, Custom
            Size (Lets you change the height of the character, good for making different aged characters)
            Scale (Lets you scale the character to your enviroment)
            
        Head Properties:
            Inherit Rotation (Toggles if the head's rotation is inherited from the chest)
            Facial Rig (Toggle the facial features of the rig on or off)
                Mouth:
                    Shape:
                        Normal, Square
                    Teeth Color
                Eye:
                    Depth
                    Color:
                        Left Eye, Right Eye
                Pupil:
                    Height
                    Style:
                        None, Normal, Cartoon
                    Color:
                        One Color, Two Color
                        Right Upper, Left Upper, Right Buttom, Left Buttom
                Eyebrow:
                    Depth
                    Height
                    Eyebrow Color
            
        Arm Properties:
            Stretch Length (The length the arms will stretch, "0.000" turns off stretch)
            Model (Alex and Steve arm models)
            Bend Types (Change the shape or way the arms bends)
            
        Leg Properties:
            Stretch Length (The length the legs will stretch, "0.000" turns off stretch)
            Fancy Feet
            Bend Types (Change the shape or way the legs bends)
            
        Armor:
            Random (Selects a random set of armor)
            3D Armor (Toggles if the armor is extruded or not)
            
            Head:
                None, Leather, Iron, Gold, Diamond, Chain
            Chest:
                None, Leather, Iron, Gold, Diamond, Chain, Elytra
            Legs:
                None, Leather, Iron, Gold, Diamond, Chain
            Feet:
                None, Leather, Iron, Gold, Diamond, Chain
                
        Extra:
            Cape: None, Custom..., Mojang Classic, Mojang, Minecon 2011, Minecon 2012, Minecon 2013, 
                Minecon 2015, Minecon 2016, Realms Mapmaker, Mojira Moderator, Colbalt, Scrolls, 
                Millionth Customer, Prismarine, Translator, Translator Chinese, cheapsh0t, 
                dannyBStyle, JulianClark, MrMessiah, Christmas 2010, New Years, Bacon
            Hat:
                None, Christmas, Fedora, Top Hat, Baseball Cap
            
Known Bugs:
    Smooth bends do not work with 3D layers enabled
    Smooth bends may distort with different rig styles
    Stretch is distorted when using blender 2.78+
    Append a second rig in a single instance of blender 2.78+ may crash or fail to append properly.
        Work Around: After each time you append the rig, save your project and restart blender before appending another one.
    
FAQ:
    
Q:"I do not see the Custom UI?"
A:"Make sure you Enable Auto Run Python Scripts in the User Preferences.  
    Make sure you have the Rig's Armature selected.  
    If you imported the rig into your own project file make sure 
    to append 'Timy Minecraft Rig.py' and run the script"
       
Q:"Why does it take a long time to render?"
A:"The lighting in this File is designed for quality and not performance.  
    If you have a graphics card in your system the make sure 
    GPU Rendering is enabled in the User Preferences and select in the
    render settings.  To Improve performance try reducing the amount of 
    samples used and lower the amount of light bounces you are using."
      
Q:"Why do I see black artifacts when I render while using 3D Layers?"
A:"Make sure the Tranparency Min and Max under Light Paths are at a higher 
    number then usual.  The 3D Layers also extrude Transparent Pixels so there 
    are alot of transparent faces your light is passing through.
    I find that 32 Min and Max is a good number to use"