---
title: "spring boot filter"
layout: post
date: 2019-02-17 12:48
tag: javascript
category: blog
author: martindelophy

---
关于spring boot 过滤器  
```
public class TestFilter implements Filter {
  @Override
  public void init(FilterConfig filterConfig) throws ServletException {
 
  }
 
  @Override
  public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain)
      throws IOException, ServletException {
    System.out.println("TestFilter");
  }
 
  @Override
  public void destroy() {
 
  }
}
```
```
	@Bean
 public FilterRegistrationBean testFilterRegistration() {
 
   FilterRegistrationBean registration = new FilterRegistrationBean();
   registration.setFilter(new TestFilter());
   registration.addUrlPatterns("/*");
   registration.addInitParameter("paramName", "paramValue");
   registration.setName("testFilter");
   registration.setOrder(1);
   return registration;
 }
```
