1.tomcat 访问jsp的流程
  jsp本质是个servlet,会在work文件夹下面生成一个servet*.java 文件，然后处理后，生成一个动态的html文件返回到前端
  类似以下：
    out.write("\r\n");
        out.write("<!DOCTYPE html PUBLIC \"-//W3C//DTD HTML 4.01 Transitional//EN\" \"http://www.w3.org/TR/html4/loose.dtd\">\r\n");
        out.write("<html>\r\n");
        out.write("<head>\r\n");
        out.write("    <meta http-equiv=\"Content-Type\" content=\"text/html; charset=UTF-8\">\r\n");
        out.write("    <title>Insert title here</title>\r\n");
        out.write("</head>\r\n");
        out.write("<body>\r\n");
        out.write((java.lang.String) org.apache.jasper.runtime.PageContextImpl.proprietaryEvaluate("${1 * 2}", java.lang.String.class, (javax.servlet.jsp.PageContext)_jspx_page_context, null));
        out.write("\r\n");
        out.write("</body>\r\n");
        out.write("</html>");
 