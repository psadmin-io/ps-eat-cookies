# ps-eat-cookies
PeopleSoft servlet filter that prevents unwanted Cookies, like PS_TOKEN.

# Setup
1. Place the sdk directory someplace that makes sense, like PS_CUST_HOME.
2. Place the classes directory in PS_CFG_HOME. `%PS_CFG_HOME%/webserv/[domain]/applications/peoplesoft/PORTAL.war/WEB-INF/classes`
3. Copy the text from template-web.xml and place in the web.xml, change as needed. `%PS_CFG_HOME%/webserv/[domain]/applications/peoplesoft/PORTAL.war/WEB-INF/web.xml`
4. Bounce the web server.
 
# Parameters
Set these parameters with the filter setup in the web.xml file.
## logFence
- 0 - minimal details
- 1 - all details

## cookiesToEat
- Comma delimited list of unwanted Cookies. `PS_TOKEN,PS_TOKENEXPIRE`

# MIT License

Copyright (c) 2016 psadmin.io

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
