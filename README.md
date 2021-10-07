# The AWL Paul V2 
## 3D printable computer keyboard with custom PCB

<img src="https://user-images.githubusercontent.com/47219621/136241411-c3836570-45db-4e9c-ad1a-863459219010.jpg" width="504" height="283.5">

The AWL Paul V2 is a follow on from my original 3D printed Alice style keyboard that was gasket mounted and handwired.
In setting out to design the V2 I had some improvements and additions I wanted to include:
- Not require painting or post processing
- Decrease the complexity of the design
- Improve the Acoustic properties of the case
- Not require soldering
- Be more accesible in general to people who come from either the MK or the 3DP community

Any questions or for sales please contact me on Discord at Alfie#6783!

The final/current version includes:

- Hotswappable PCB with a rotary encoder and USB C
- Leaf springs - similar to the salvation keyboard
- '1-Piece' case design - no sandwich panels
- Wrist rest designed just for the board
- Low profile design so can be used without the rest

This GitHub repo will hopefully contain all the current and past STLs to print the case, plate and wrist rest as well as some DXFs that may be used to cut foam for between the plate and PCB if wanted.

## Layout
The layout is similar to the popular Alice layout with an inward angled alpha section at 8 degrees. In addition, there is a rotary encoder, 2 macro keys and an arrow clustered on the right of the board. Left ALT and Control are shifted left to allow the arrow cluster to sit more closely and reduce the boards footprint. A 1u right shift is adopted here and can be replaced with a spare upwards arrow. The board also has 2 B keys. Overall the layout tries to adopt the general and most available sizes for keycaps such as Tab, Capslock, Left Shift and Control and Windows key however the bottom row uses a 2.25 and 2.75 space/ backspace key and 1u Fn, Alt and Control.

## Design of Case

The case design is quite simple with the aim of being simple and embracing the way in which cases often are assembled. The design allows for the PCB to be dropped into the case  and attached to cantilevers using 2 M2 screws and then in order to ensure that the keycaps are nicely conformed to, two covers are screwed in from the front. One of these covers are central and bridges the PCB across the middle, hugging the keycaps on either half of the board. One of the covers is on the right and 'clips' into the case next to the arrows; it worms around the arrow keys and between the RHS of the board and the macro row on the right and finishes up around the rotary encoder. This cover is affixed using 3 screws, 2 above the rotary encoder and 1 above the arrows. Due to this design these 6 screws are on show and as such you may want to select the finish on them to match the case and the keycaps you choose.

The case is made to be as small as possible without excessive borders in its attempt at an industrial yet functionally minimal design. The wrist rests hugs the front of the case with only a chamfer to seperate the two items. 

The case has feet that are formed from rubber bumpons at the front and at the rear. If you want the board to sit at an angle then you can screw in some feet at the rear. Currently options are available to allow the case to sit at either 0 degrees, 3 degrees or 6 degrees.

Under the PCB the case has integrated cantilevers that operate similarly to leaf springs found in other boards. 2 of the outer cantilevers have M2 brass inserts and are used to affix the pcb to the case while the remaining posts on the other cantilevers just have a 6mm foam pad that provides a more even and soft feel. Damping remains a function of the intrisic material properties of the cantilver and little to no vibrations or additional noises are observed. The user can choose to affix thicker or thinner foam or miss some post locations in order to alter the feel of the board to make it more or less stiff and introduce more flex if desired. 

## Design of PCB
The PCB uses an Atmega32u4, USB C with proper anchoring and an Alps EC11 Rotary Encoder footprint (not necessarily ALPs). The board is hotswappable and uses screw in stabilisers and rests on up to 12 mounting points.

## Availability and Cost

For now, the PCB will be available for sale from myself through Discord using Paypal business invoices as well as the option to purchase the hardware, a printed case or a complete keyboard and wrist rest set. These prices are subject to change and any hardware I sell alone is sold at cost to me (I don't make any money) when purchased with a pcb:

| Item              | Description | Price |
| -----------       | ----------- | ----- |
| PCB               | Soldered PCB              | £35.00 |
| PCB + Hardware    | Soldered PCB + Screws, Inserts, Foam Pads, Feet, Magnets (Optional)            | £45.00 / £50.00 |
| Case + PCB        | PCB with assembled case - just add switches, stabs and keycaps             | £125.00 |
| Case + Wrist Rest + PCB              | As above but with magnets              | £165.00 |

The hardware included when sold / needed to have a complete case is as follows and is for the latest release and is the bare minimum - i.e. you may choose brass or black oxide screws for the front facing screws:
- 6 x M3x10 Cap Head screws (for front covers)
- 2 x M3x8/10 Cap head screws (for feet)
- 2 x M3x14 Cap Head screws (for joining 2 halves)
- 2 x M2x5/6 Cap head screws (for pcb attachment)
- 2 x M2 Washers (Optional but recommended)
- 10 x M3 Brass Inserts (OD: 3.9-4.2mm | Len:4-6mm) (See Section)
- 4/12 8mm Rubber Bumpons (Good to have more. At least 4/12 needed for case/wrist rest)
- 10 x 6mm Foam Pads (2mm - 2.5mm thick)(For the posts/PCB interface. More are supplied)

## Notes on Brass Inserts
The holes in the design that recieve brass inserts are 3.9mm in diameter and vary in length. The case was designed for brass inserts that were 4.1mm in length and meant to have holes that were 3.7mm to 4.0mm. For guidance these brass inserts measure as being 4.28mm at a maximum OD and 3.7mm at their smallest OD. They look like this:

<img src="https://user-images.githubusercontent.com/47219621/136241462-da60718c-6437-4915-9537-aefa999eb399.jpg" width="281" height="208">


Most M3 Brass inserts will do that are between 4mm to 6mm in length. They may simply require more or less heat/pushing to set them in and some clean up in the form of a tap or knife to remove any plastic in the way of the threads. The important part is that they sit slightly below the surface they are located on and that a bolt, when screwed in, is perpendicular to said surface. Some common sense may need to be applied when choosing and installing inserts :p. All inserts should be tested before final assembly by test fitting a bolt and seeing if they pull out with reasonable force. If they do then they may need to be reset in the hole and possible have some additonal plastic melted into the hole or over the insert to hold it in place.

## Notes on Printing and Settings
For printing parts I use 3 seperate profiles, one for the case parts, one for the wrist rest parts and one for the knob. I will post screenshots and config bundles for use with the Prusa i3 Mk3s and Prusa Slic3r that I use however note that profiles will not necessarily transfer, even to the same model of printer. In general you should follow for the case printing:

- PLA will provide good detail and adequate strength (Springs are also designed for PLA's stiffness)
- 0.3mm first layer height (If not done for the case this is needed to ensure the layers add up to 1.5mm for the plate)
- 0.2mm layer height for everything else
- 5 Perimeters
- 5 Top layers
- 5 Bottom Laers
- 35% Rectilinear Infill
- Seems should be ALIGNED and I tend to paint them on areas of the models that wont be seen in normal use (in between case parts etc)
- I use Slic3rs Monotonic infill for a better surface finish
- Detect thin walls and compress traces down to one perimeter or gap fill is needed in some areas to avoid marks on the outside of the case. This is prevalent where the screw enters the front of the RHS case part for joining the cases.
- Supports aren't required or recommended anywhere.
- When printing PLA you need to experiment with the fan and temperature settings to ensure that minimal curling / warping will occur. The nature of the case makes is susceptible to warping at the corners. You may choose to add pads or a brim but this adds to cleanup and could alter the aesthetics of the design.

For the Wrist Rests I reduce the bulk as it is not acoustically vital and saves on filament and print time:
- Reduce bottom layers to 3
- Reduce top layers to 4
- Reduce perimeters to 3
- Reduce infill to 15% (this is optional but can save filament)

For the Knob I use a near identical profile to the case but just with 0.1mm layer heights to increase the quality of the feel.

## Post Processing and other issues
Depending on the encoder used and other variables related to the 3D printing of the encoder knob, the fitment may not be as desired (firmly attached to post but can be removed by hand). In order to fix this you can experiment with scaling the knob in small intervals (a 0.1mm to 0.2mm can be all the difference) or you can use a knife or hot metal object to slightly deform the internal hole of the knob to make it more or less firmly affixed.
