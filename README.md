# SpringCard Web PC/SC SDK

This is the SDK published by SpringCard to access smart cards and PC/SC readers from a web page.

## A short introduction

Back in the old times, when Internet Explorer ruled the world, a few companies (including us!) have developed ActiveX components to make it possible for a JavaScript application, running inside the web browser, to communicate with a smart card, a contactless card or a RFID label, either through the system's PC/SC middleware or through a more proprietary solution.

When the need for portability and the security of the ActiveX objects have become a concern, another few companies (yet we were still in!) have developed Java Applets designed for the same purpose: creating a "bridge" between a web page, served by a remote server, and a local token, credential or identication object. For many years, embedding Java's `javax.smartcardio` in an Applet has been <u>the</u> solution to "do" PC/SC in the browser.

Once again, security requirements have been dramatically raised, and modern web browsers have for long removed the support of the Java plug-ins system. The deprecation of the Applet API in 2016 ([JEP 289](https://openjdk.java.net/jeps/289)), and its removal from Java specifications in 2020 ([JEP 398](https://openjdk.java.net/jeps/398)) have been the last nails in the coffin.

Anyway a lot of application-providers are still looking for a solution to bridge their web application with PC/SC readers and smart cards. Think for instance of a full-cloud POS software, or an hotel-management SaaS application, that needs to read loyalty cards, or to encode access cards on-the-fly. Think also of a web-based corporate or school applications, where the ability to access the employee's or student's badge would dramatically simplify the user experience, without the complexity and the price of a complete SSO solution.

SpringCard's response to this need is SpringCard Companion, a light-weight, "invisible" application that exposes PC/SC readers -- and other SpringCard devices -- through a REST API and a WebSocket. Provided that the browser's policy allows the web content to connect to `localhost` (`127.0.0.1`), the JavaScript programs may again access smart cards, contactless cards and RFID labels in a seamless way.

This SDK contains a set of very-basic sample web-applications (HTML + JavaScript) to get off to a good start with SpringCard Companion in no time.

**Just follow the steps:**

1. Install latest version of SpringCard Companion Service (SN20030) from [www.springcard.com/download/find/file/sn20030](https://www.springcard.com/en/download/find/file/sn20030),
2. Discover the sample web-applications live on [demo.springcard.com/web-pcsc](https://demo.springcard.com/web-pcsc),
3. Clone this SDK and create your own application(s) based on the source code of these applications.

## Legal disclaimer

THE SDK IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.

## License

This software is part of SPRINGCARD SDKs

Redistribution and use in source (source code) and binary (object code) forms, with or without modification, are permitted provided that the following conditions are met :

1. Redistributed source code or object code shall be used only in conjunction with products (hardware devices) either manufactured, distributed or developed by SPRINGCARD,
2. Redistributed source code, either modified or un-modified, must retain the above copyright notice, this list of conditions and the disclaimer below,
3. Redistribution of any modified code must be clearly identified "Code derived from original SPRINGCARD copyrighted source code", with a description of the modification and the name of its author,
4. Redistributed object code must reproduce the above copyright notice, this list of conditions and the disclaimer below in the documentation and/or other materials provided with the distribution,
5. The name of SPRINGCARD may not be used to endorse or promote products derived from this software or in any other form without specific prior written permission from SPRINGCARD.

Please read to `LICENSE.TXT` for the complete license statement. Please always place a copy of the `LICENSE.TXT` file together with the redistributed source code or object code.

## How to contact us

Retrieve all our contact details on [www.springcard.com/contact](https://www.springcard.com/en/contact).
