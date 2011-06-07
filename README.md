YQL-ACCESSIBILITY
=================
This project aims at implementing a unified interface to generate XML reports on accessibility issues of web sites. The idea is to use YQL capabilities for getting accessibility reports from automatic accessibility evaluation tools and provide a single interface for acessing these data.

XML RESPONSE LAYOUT
-------------------

The base XML structure being used in this projects presents the following data layout:
    &lt;result&gt;
        lt;error&gt;
          lt;priority&gt;Priority 1lt;/priority&gt;
          lt;checkpoint&gt;1.1lt;/checkpoint&gt;
          lt;description&gt;Text descriptions for the errorlt;/description&gt;
          lt;lines&gt;9lt;/lines&gt;
        lt;/error&gt; 
        lt;warning&gt;
          lt;priority&gt;Priority 1lt;/priority&gt;
          lt;checkpoint&gt;4.1lt;/checkpoint&gt;
          lt;description&gt;Text descriptions for the warninglt;/description&gt;
          lt;lines&gt;1lt;/lines&gt; 
        lt;/warning&gt;
    lt;/result&gt;

These data are encapsulated in a YQL XML formated response from the service, and can be retrieved as XML or JSON text messages. If you would like to get more information on YQL, take a look at: http://developer.yahoo.com/yql/.

AVAILABLE TABLES
----------------

For the time, we have only two available tables:
# EvalAccess 2.0: http://sipt07.si.ehu.es/evalaccess2/
# DaSilva: http://www.dasilva.org.br/
