Screw Helix Sheet Metal Expansion Macro

This project contains a SolidWorks VBA macro that creates a flat pattern (planification) for a screw conveyor flight. The user can enter the key parameters of the helix through a custom userform. The macro calculates the geometry, builds the sketch, trims the profile, adds dimensions, and generates a sheet metal base flange with the correct thickness and bend allowance.

The goal of this macro is to make the process of creating flat patterns for screw flights fast, repeatable, and less dependent on manual sketching. It may be useful for mechanical designers, fabrication companies, and SolidWorks users who work with screw conveyors or auger systems.

Features

The macro asks the user to enter the outer diameter, inner diameter, pitch, and thickness. All values are validated to avoid negative numbers or invalid inputs. The program also detects if the user closes the form using the X button and cancels the entire macro safely.

The macro searches the feature tree to find the Front, Top, and Right planes in a language-independent way. This avoids problems when SolidWorks is installed in different languages.

After reading the inputs, the macro calculates the inner and outer helix lengths, the eccentricity, the radii needed for the flat pattern, and the sweep angle that defines the arc of the sheet. It then creates the circles and radial lines, trims the sketch to form the correct profile, applies dimensions, and adds a sheet metal base flange.

Requirements

This macro must be used in SolidWorks. It was tested using VBA inside the SolidWorks macro editor. The code should work in most modern versions of SolidWorks, as long as sheet metal features are available.

Usage

Open SolidWorks and open or create a blank part. Load the macro from Tools > Macro > Run. Enter the required dimensions in the userform and click Confirm. The macro will build the full flat pattern automatically. If the user closes the form, the macro stops without making changes.
Only the ScrewHelixFlatPattern.swp file is necessary to run the generator.

Files included

The VBA macro file with the full code.
The userform with all input fields and validation.

Notes

This macro is not an exact engineering calculator for all situations. The geometry produced is based on a simple mathematical method to approximate a screw flight development, which is suitable for many practical manufacturing cases. Users should always confirm if the generated flat pattern matches their workshop requirements.
