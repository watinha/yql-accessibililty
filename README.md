YQL-ACCESSIBILITY
=================
This project aims at implementing a unified interface to generate XML reports on accessibility issues of web sites. The idea is to use YQL capabilities for getting accessibility reports from automatic accessibility evaluation tools and provide a single interface for acessing these data.

XML RESPONSE LAYOUT
-------------------

The base XML structure being used in this projects presents the following data layout:
> <result>
>     <error>
>       <priority>Priority 1</priority>
>       <checkpoint>1.1</checkpoint>
>       <description>Text descriptions for the error</description>
>       <lines>9</lines>
>     </error> 
>     <warning>
>       <priority>Priority 1</priority>
>       <checkpoint>4.1</checkpoint>
>       <description>Text descriptions for the warning</description>
>       <lines>1</lines> 
>     </warning>
> </result>

These data are encapsulated in a YQL XML formated response from the service, and can be retrieved as XML or JSON text messages. If you would like to get more information on YQL, take a look at: http://developer.yahoo.com/yql/.

AVAILABLE TABLES
----------------

For the time, we have only two available tables:
# EvalAccess 2.0: http://sipt07.si.ehu.es/evalaccess2/
# DaSilva: http://www.dasilva.org.br/
