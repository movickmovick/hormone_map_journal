Hormone Map

name Cortisol
shape Rectangle
color Teal
outputs Enkephalins, Glucose, Endorphins, POMC, alpha-MSH, ACTH, POMC
inputs NPY
description "The stress hormone"
class glucocorticoid

name NPY
shape Rectangle
color yellow
outputs cortisol, ACTH, Leptin, CRH, 
inputs stress, CRH, fasting, Leptin, Insulin, Canabinoids, 
description "vasoconstrictor"
class peptide

name ACTH
shape Rectangle
color Teal
outputs Epinephine, Norepinephrine
inputs NPY, Cortisol, CRH
description "messenger"
class polypeptide

name Epinephine
shape Rectangle
color Teal
outputs Leptin, Glucose
inputs ACTH
description "flight or flight hormone"
class organic_chemical

name glucose
shape elipse
color teal
outputs none;
inputs Adiponectin Insulin resistance Insulin Testosterone Glucagon Epinephrine Cortisol 
description recieved in the hypothalamus
class monosaccharides

name nitrosamine 
shape elipse
color green 
outputs insulin receptor (muscle cell)
inputs none
description "the cancerous meat one" 
class organic_compound
question what is a nitrate because a nitrosamine is formed when a protein reacts with a nitrate

name ocytocin
shape rectangle
color green
outputs insulin insuling_receptor
inputs none
description "the feel good hormone"
class "G-protein-coupled receptor"

name insulin
shape rectangle
color green
outputs insulin_receptor,  insulin_receptor(1), Testosterone, Glucose, HGH, 
inputs PP, GIP, Oxytocin, GLP-1, HGH
description "pancreas production
class 

name Glucose-dependent insulinotropic polypeptide (GIP)
shape rectangle
color blue
outputs Insulin, Glucogen
inputs none
description "K-cell and large intestine secretion"
class polypeptide


name GLP-1
shape rectangle
color green
outputs Insulin, Glucagon
inputs Acetate3, Propiate
description "L-cell secretion"
class peptide

name Leptin
shape rectangle
color blue	
outputs Leptin receptor, NPY, Insulin Receptr (muscle), Insulin Receptor (Liver), CART, AGRP, MCH, Brown Fat Cell, Alpha-MSH, 
		Adiponenctin, Orexins, Canabinoids, Thyroid Hormones, Brown Fat Cell,  
inputs NPY, Epinephrine, Brown Fat Cell (?), Testosterone, 
description "makes cells more sensitive to insulin"
class hormone

name NPY
shape rectangle 
color Yellow	
outputs Leptin, CRH, ACTH, Cortisol
inputs CRH, Leptin, Insulin, Canabinoids, Stress, Fasting, 
description "36-amino acid peptide with many functions"
class peptide


name CRH
shape rectangle 
color Blue	
outputs POMC, NPY, Enkephalins, ACTH, Endorphins
inputs Leptin, NPY
description "41-amino acid peptide produced in reponse to stress"
class Corticotropin-releasing hormone

name Dopamine
shape rectangle
color teal
inputs Ghrelin, Canabinoids, CART
description functions as a nuerotrasmitter
class organic_chemical

name Ghrelin
shape rectangle
color yellow
inputs OXM, Glucagon, Fasting, Insulin,
outputs Dopamine, Insulin, HGH, CART, AGRP
description "hunger hormone": produced by enteroendocrine; 
class hormone
question "Knowing its role, Stimulate appetite, slow your metabolism, and increase your fat storage
	   how does Ghrelin achieve this? What is the structure made of, seeing that it is a functional
	   hormone? Are the four inputs fed through simultaneously or concurrently? Similarly what
	   is the timing of the outputs.

name CART
shape rectangle
color blue
inputs Ghrelin, Leptin
outputs alpha-MSH, POMC
description Interacts with dopamine circuits in the brain that control desire, craving, reward, addiction.
class peptide
question "Knowing Ghrelin is the 'hunger hormone' and CART interacts with the circuits that involve
	  craving, reward, addiction, etc., what are their similarities? How are the different?"

name AGRP
shape rectangle
color yellow
inputs Ghrelin, Leptin, Stress
outputs alpha-MGH, MC4R
Description Hypothalymus sender
Class hormone
question what is a better description for AGRP? on page 129 of Smith's Gut Reactions there is a 
	  a diagram depicting its station withint the Hypothalamus' Arcuate nucleus. How come
	  it has to be paired up with NPY? How come the hypothalumus controls appetite?
quote "The hormone that AGRP blocks is alpha-melanocyte-stimulating hormone (alpha-MSH)
quote "Inflamation increase AGRP, which increases inflamation."

name alpha-MSH
shape rectangle
color blue
inputs Leptin, CART, POMC, Corisol
outputs none
Description Several Functions: protects the brain from infalmation. regulate melanin pigment in skin and 	      hair, sebum secretion, temperature regulation, pain control, sex behaviors, learning...
class hormone

name Cortisol
class ?

name GLP-1
class peptide
description "decreases hunger by slowing acid release into the stomach, and slows the emptying of the stomach"
shape rectangle
color teal
inputs acetate, Propionate
outputs Insulin, Glucagon

name Glucagon
class hormone
description "The glucose (loci: liver) accelerator pedal; produced in the pancreas by the alpha cells; appetite suppressant; reduces ghrelin"
shape rectangle
color blue
inputs GIP, GLP-1, OXM, fasting
outputs Ghrelin, Glucose

name OXM
class peptide
description "secreted, like GLP-1 and PYY, when food is ingested and it is secreted in proportion to the calories consumed; it acts as a satiety signal;
	     OXM, or Oxynyomodulin reduceds the hunger hormone ghrelin"
shape rectangle
color blue
inputs none
outputs ghrelin, glucagon, insulin

name CCK
class unknown
description related to the eating system where it relates to hunger suppression. when you fast this kicks in.
shape rectangle
color blue
inputs PP
outputs none

name PP
class unknown
description kicks in when fast and accelerates towards CCK; pings on the same lines as Glucagon and Ghrelin;
shape rectangle
color blue
inputs fasting
outputs CCK

name fasting
description "human control factor"
shape elipse
color grey
inputs none
outputs Glucagon, PP, Leptin Receptor (Fat cell);

name stress
description "human control factor"
shape elipse
color grey
inputs none
outputs AGRP, NPY

name excercise
description "human control factor"
shape elipse
color grey
inputs none
outputs Irisin, insulin receptor(Muscle Cell)

name fiber
description "human control factor"
shape elipse
color grey
inputs none
outputs Gut-Microbes

name Gut-Microbes
description "human control factor (?)"
shape elipse
color grey
inputs Fiber
outputs Acetate, Propionate

name Acetate 
shape elipse
color green 
outputs PYY
inputs Gut-Microbes
description "messenger"; acetate may regulate appetite possibly through central hypothalamic mechanisms 
			and satiety through acetate-induced or gut hormone-induced vagal activation.
class salt formed with acetic acid and a base; helps to keep your gut environment stable
question how come acetate reacts violently?

name PYY
description active function when the body isn't eating, thinking of eating (?); relays; 
shape rectangle
color blue
inputs fasting, acetate, Propiate
outputs none
class gut-hormone

name HGH (Human Growth Hormone)
shape rectangle 
color green
description Pitutitary production (brain base); accelerates fat loss; 
class hormone
inputs sleep_deprivation, Alcohol, Ghrelin, insulin;	
outputs insulin, IGF-1;

name IGF-1
shape ellipse
color green
description insulin growth factor that spurts growth in puberty; binds to the insulin receptor, only 1 percent.
class hormone
inputs HGH. why? 
outputs vitamin D3

name Irisin
shape rectangle
color Irisin
description hormone produced when excercising
class hormone
inputs excercise
outputs Brown_Fat_Cells

name Brown_fat_cells
shape white
color square
description
inputs Irisin, Cold_exposure, Polyphenols, Orexins, Leptin;
outputs none (?)

name Orexins
shape rectangle
color teal
description
inputs
outputs


