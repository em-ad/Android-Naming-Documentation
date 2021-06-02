# Android-Naming-Documentation

### 1.	Class File names should be UpperCamelCase and extended component should be at the end of name. examples: `SignInActivity`, `UserProfileModel`, `BaseDialog`, `NetworkViewModel`
### 2.	Resource Files should be `snake_case` with component at the start of the name and the option (or special state) at the end of the name. examples: `item_profile_vertical`, `fragment_requests`, `button_accept_pressed`, `button_accept_selected`
#### a.	Icon recourses: `ic_name`
#### b.	Drawables extending a class: `text_view_name`
#### c.	Don’t use words ‘menu’ and ‘drawable’ because they are in that folder
### 3.	Braces: 
#### a.	no {braces} for short single line conditions without else
#### b.	Line Break after opening brace {
#### c.	No Line Break before opening brace
#### d.	Line Break before closing bracket
#### e.	Line Break after closing bracket (except for else)
#### f.	Empty blocks should not be in single line. { } is bad
### 4.	Each Line should normally have at most 100 characters
#### a.	Exception 1: Literal Strings can be in a single line (like url)
#### b.	Package name and import lines can be in a single line
#### c.	Commands in comments that are parsed by shells
### 5.	Line Break: 
#### a.	Break lines before operators like dot, double colon,
#### b.	Don’t break lines before braces ( )
#### c.	Don’t break lines before comma ,
#### d.	Don’t break lines before lambda ->
### 6.	Nullability in kotlin: Never use `!!` and don’t use `?` too much. Add logical null prevention instead.
### 7.	Exception: 
#### a.	Never ignore exceptions in code (do something in catch)
#### b.	Don’t use generic exceptions. For example, don’t use `Exception` when you can use `NullPointerException`.
### 8.	GC: don’t customize finalization process. If you need to use finalizer or closer, add complete comment and doc for your reason
### 9.	Detailed Imports Only: Don’t use full packages. Example: `import lib.*` is bad. Use import `lib.used_section`
### 10.	Field (Object) definition:
#### a.	Private and non-static objects can begin with “m”
#### b.	Private and static objects can begin with “s”
#### c.	Final static constants should be ALL_UPPER_CASE. Example: `KEY_INTENT_IMAGE`
### 11.	Acronyms are named like words. Example: `LocationAPI.java` and `XMLHTTPRequest` is wrong! Use `LocationApi.java` and `XmlHttpRequest`
### 12.	Don’t use `@SuppressWarnings` unless it is absolutely necessary. Don’t ignore warnings either.
### 13.	Annotations for classes and functions should be separate lines. Annotations for fields (objects) should be all before the field in 1 line (unless 100 char is exceeded)
### 14.	Scoping: each variable should be defined in the inner most scope available. For local variables, they should be instantiated before their usage. If it’s possible, initialize every variable when defining
### 15.	Imports should be in 4 groups with one empty line between them. And sort in each group is alphabetical:
#### a.	Android Imports
#### b.	3rd Party Libraries
#### c.	Java and Javax libraries
#### d.	Modules and same project libraries
### 16.	Logging: 
#### a.	Use class name and operation (if needed) as tag in Logging
#### b.	Disable logs for release mode
### 17.	Class Member Ordering:
#### a.	Constants
#### b.	Fields
#### c.	Constructors
#### d.	Override methods and callbacks (public or private)
#### e.	Public methods
#### f.	Private methods
#### g.	Inner classes or interfaces
### 18.	Function Call Parameter Ordering:
#### a.	Context Based Components (context, activity, lifecycle, …)
#### b.	Normal Classes
#### c.	Interfaces and Callbacks
### 19.	Constants Naming should start with section: PREF_, EXTRA_, KEY_, ...
### 20. XML:
#### a. no empty tags! if elements doesnt have inner elements, use closing xml
#### b. id: `camelCase_other_other_other`. example: `textView_profile_first_name`


##### to be continued...