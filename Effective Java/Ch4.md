# Notes

## Item 15 Minimize the accessibility of classes and methods
* Facilities to aid in **information hiding**
	* access control
		* rule of thumb: make each class or member as inaccessible as possible
		* for member, 4 possible access levels
			* $private$
			* $protected$ accessible from subclasses of the class
			* $public$ accessible anywhere
			* $package-private$ default
	* `public static final`
		* nonzero-length is always **mutable** 
		* ∴ it is wrong for a class to have a `public static final` array field 