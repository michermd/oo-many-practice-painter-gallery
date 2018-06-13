# oo-many-practice-painter-gallery

(after @aalexander3/oo-many-many-practice)

# Here's our domain:
  * Painter
  * Gallery
  * Paintings

# How is this modeled?
  * A painting belongs_to a painter
  * A painting belongs_to a gallery
  * A painter has_many paintings
  * A gallery has_many paintings
  * A painter has_many many galleries through paintings
  * A gallery has_many painters through paintings

==============================================================

# OBJECTIVES
  * Draw this domain on a whiteboard or http://awwapp.com/
  * Build out the three classes and files from scratch (keep in mind the relationships)
  * Think about how the classes will interact -- how does a doctor know about their patients?
  * Use attr_reader, attr_writer, & attr_accessor
  * Create a run file with a single point of entry
  * Maintain single source of truth for all classes

==============================================================

# DELIVERABLES
  * Gallery
    * #initialize a gallery is initialized with a name and a neighborhood in NYC
    * a gallery cannot change its name, but can change its neighborhood
    * Gallery.all returns all instances of the gallery class
    * #paintings returns an array of all the painting instances that belong_to a gallery
    * #painters return an array of all the painters that are associated with a gallery
    * #painter_names return an array of just the names of said painters (First and Last), not the full object
    * #change_neighborhood takes in a gallery and a new neighborhood and changes the gallery's neighborhood

    ====== BONUS ======
    * Gallery.find_by_neighborhood takes in a neighborhood (e.g., "gym") as an argument and finds a gallery by a given neighborhood
    * Gallery.most_paintings returns the name of the gallery (as a string) with the most paintings

==============================================================
  * PAINTER
    * #initialize a painter is initialized with a first_name, last_name, and style
    * a painter cannot change their name
    * Painter.all returns all instances of the painter class
    * #painter_name converts a member's first_name,last_name, and style to bio sentence (e.g., "John Smith", "expressionist => "John Smith is an Expressionist.")
    * #paintings returns an array of all the paintings associated with an instance of painter
    * #new_painting creates a new painting instance taking in an gallery and a title
    ====== BONUS ======
    * Painter.find_by_style takes in style as an argument and finds a painter's full name by a style
    * Painter.most_active returns the painter (as an object) with the most paintings
    
==============================================================
  * PAINTING
    * #initialize a painting is initialized with a title, a painter, and an gallery
    * an painting has corresponding methods for all three attributes
    * Painting.all returns all instances of the painting class

==============================================================
