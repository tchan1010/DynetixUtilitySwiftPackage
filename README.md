# DynetixUtilitySwiftPackage


This is a Swift Package library which contains a set of utility functions.

This package can be imported to any iOS app via the Swift Package Manager.

Once you've included the package into your iOS project: 

1. In your iOS app's Swift source files, add:

   import DynetixUtilitySwiftPackage


2. Call any of these Swift functions:

     /* ---------------------------------------------------------------------- 
        Show a user message, and optional send the message via email by 
        passing true to doEmail argument. The optional image, if specified,
        will be sent as an attachment in the email.
        ---------------------------------------------------------------------- */
     func showMessage(_ caller: UIViewController, _ title : String, _  msg : String,
                        _  doEmail : Bool = false, _ image : UIImage? = nil)



     /* ---------------------------------------------------------------------- 
        Send an email with an optional image attachement
        ---------------------------------------------------------------------- */
     func sendEmail(_ caller: UIViewController, _ subject : String, _  msg : String, _  image : UIImage? )

     Note: to send email, the 'caller' should be a MFMailComposeViewControllerDelegate


     /* ---------------------------------------------------------------------- 
        Convert the given elapsed time (in seconds) to a string that 
        depicts elapsed time in hrs, minutes and/or seconds
        ---------------------------------------------------------------------- */
     func second2Str(_ total_seconds : Int64 ) -> String


     /* ---------------------------------------------------------------------- 
        Convert a given date object to a string time stamp
        ---------------------------------------------------------------------- */
     func date2Str(_ date : Date ) -> String 
