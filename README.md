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

The final/current version includes:

- Hotswappable PCB with a rotary encoder and USB C
- Leaf springs - similar to the salvation keyboard
- '1-Piece' case design - no sandwich panels
- Wrist rest designed just for the board
- Low profile design so can be used without the rest

This GitHub repo will hopefully contain all the current and past STLs to print the case, plate and wrist rest as well as some DXFs that may be used to cut foam for between the plate and PCB if wanted.

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
