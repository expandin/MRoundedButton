MRoundedButton
==============

MRoundedButton is a subclass of UIControl and the appearance is like the iOS 7 **Phone** app button or the button on the **Control Center**

Four button styles are suplied:

    MRoundedButtonDefault           //  central text
    MRoundedButtonSubtitle          //  text with subtitle 
    MRoundedButtonCentralImage      //  central image
    MRoundedButtonImageWithSubtitle //  image with subtitle

MRoundedButtonAppearanceManager
===============================

MRoundedButtonAppearanceManager is the appearance manager for the MRoundedButton, each appearance information can be stored in an [NSDictionary](https://developer.apple.com/library/ios/documentation/Cocoa/Reference/Foundation/Classes/NSDictionary_Class/Reference/Reference.html) object with a unique identifier:

    NSDictionary *appearanceProxy = @{kMRoundedButtonCornerRadius : @40,
                                      kMRoundedButtonBorderWidth  : @2,
                                      kMRoundedButtonBorderColor  : [UIColor clearColor],
                                      kMRoundedButtonContentColor : [UIColor blackColor],
                                      kMRoundedButtonContentAnimationColor : [UIColor whiteColor],
                                      kMRoundedButtonForegroundColor : [UIColor whiteColor],
                                      kMRoundedButtonForegroundAnimationColor : [UIColor clearColor]};
    [MRoundedButtonAppearanceManager registerAppearanceProxy:appearanceProxy1 forIdentifier:#<UNIQUE_IDENTIFIER>];
    
MRHollowView
============

MRHollowView can be used to place the MRoundedButton on an image view or something.
> In the drawRect: method, each subview of HRHollowView are EO cliped to its bounds. Then the superview content can be displayed via the hollowed shapes.
    
TODO
====
1. Fix typo (I'm not a native English speaker, so I need your help)
2. Border issue
3. Make it Cocoapods
    
Lisence
=======
> Permission is hereby granted, free of charge, to any person obtaining a copy
> of this software and associated documentation files (the "Software"), to deal
> in the Software without restriction, including without limitation the rights
> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
> copies of the Software, and to permit persons to whom the Software is
> furnished to do so, subject to the following conditions:
>
> The above copyright notice and this permission notice shall be included in
> all copies or substantial portions of the Software.
>        
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
> THE SOFTWARE.
        
