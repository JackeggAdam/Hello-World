





<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
  <link rel="dns-prefetch" href="https://github.githubassets.com">
  <link rel="dns-prefetch" href="https://avatars0.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars1.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars2.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars3.githubusercontent.com">
  <link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com">
  <link rel="dns-prefetch" href="https://user-images.githubusercontent.com/">



  <link crossorigin="anonymous" media="all" integrity="sha512-5Bs4ERl99/u2AUfpOZF2F0cdfNby7+Vd9teUshXUBPo5CjwECR7IAEf+weI/eCk5tF7K1h3O8hd8k0+P/HePeg==" rel="stylesheet" href="https://github.githubassets.com/assets/frameworks-e41b3811197df7fbb60147e939917617.css" />
  <link crossorigin="anonymous" media="all" integrity="sha512-21eX2YaEYIYa91WFh0mXaxJ3wLQxy2ldlpRbyuCueK3MvqHGEzmXYPkMQ4XBtASauZXKlL1hPxQQU9g28R03wQ==" rel="stylesheet" href="https://github.githubassets.com/assets/site-db5797d9868460861af755858749976b.css" />
    <link crossorigin="anonymous" media="all" integrity="sha512-FwYpFVuVzDWMuKKB1OvzQkN/OMqH9BH+TbbPuFsu+TxHn58kX+dB37udsPZSBrQaBCX8s1kPyd1k8B8d2/o/qQ==" rel="stylesheet" href="https://github.githubassets.com/assets/github-170629155b95cc358cb8a281d4ebf342.css" />
    
    
    
    


  <meta name="viewport" content="width=device-width">
  
  <title>sql_node/MySQL学习笔记.md at master · hjzCy/sql_node · GitHub</title>
    <meta name="description" content="sql学习笔记。. Contribute to hjzCy/sql_node development by creating an account on GitHub.">
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
  <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
  <meta property="fb:app_id" content="1401488693436528">

    <meta name="twitter:image:src" content="https://avatars2.githubusercontent.com/u/39392770?s=400&amp;v=4" /><meta name="twitter:site" content="@github" /><meta name="twitter:card" content="summary" /><meta name="twitter:title" content="hjzCy/sql_node" /><meta name="twitter:description" content="sql学习笔记。. Contribute to hjzCy/sql_node development by creating an account on GitHub." />
    <meta property="og:image" content="https://avatars2.githubusercontent.com/u/39392770?s=400&amp;v=4" /><meta property="og:site_name" content="GitHub" /><meta property="og:type" content="object" /><meta property="og:title" content="hjzCy/sql_node" /><meta property="og:url" content="https://github.com/hjzCy/sql_node" /><meta property="og:description" content="sql学习笔记。. Contribute to hjzCy/sql_node development by creating an account on GitHub." />

  <link rel="assets" href="https://github.githubassets.com/">
  
  

  <meta name="request-id" content="AAD8:741E:FDCE62:1512EE7:5E6B78C3" data-pjax-transient="true"/><meta name="html-safe-nonce" content="e3c52fb236165a320da8d462c714492abcda8b01" data-pjax-transient="true"/><meta name="visitor-payload" content="eyJyZWZlcnJlciI6Imh0dHBzOi8vd3d3LmJpbGliaWxpLmNvbS92aWRlby9hdjM5ODA3OTQ0P2Zyb209c2VhcmNoXHUwMDI2c2VpZD0xMjMxMDk2OTQ2NTEyNTcxODAyNSIsInJlcXVlc3RfaWQiOiJBQUQ4Ojc0MUU6RkRDRTYyOjE1MTJFRTc6NUU2Qjc4QzMiLCJ2aXNpdG9yX2lkIjoiMTY4OTk2MDk0ODQxMjY3NjI5MiIsInJlZ2lvbl9lZGdlIjoiYXAtc291dGhlYXN0LTEiLCJyZWdpb25fcmVuZGVyIjoiYXAtc291dGhlYXN0LTEifQ==" data-pjax-transient="true"/><meta name="visitor-hmac" content="c8ecb05c7855d7c52d000d543cf7f26661a0cc95b9ef33cba0c7b994e8a587d9" data-pjax-transient="true"/>



  <meta name="github-keyboard-shortcuts" content="repository,source-code" data-pjax-transient="true" />

  

  <meta name="selected-link" value="repo_source" data-pjax-transient>

      <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
    <meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-site-verification" content="GXs5KoUUkNCoaAZn7wPN-t01Pywp9M3sEjnt_3_ZWPc">

  <meta name="octolytics-host" content="collector.githubapp.com" /><meta name="octolytics-app-id" content="github" /><meta name="octolytics-event-url" content="https://collector.githubapp.com/github-external/browser_event" /><meta name="octolytics-dimension-ga_id" content="" class="js-octo-ga-id" />
<meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" />



    <meta name="google-analytics" content="UA-3769691-2">


<meta class="js-ga-set" name="dimension1" content="Logged Out">



  

      <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

      <meta name="expected-hostname" content="github.com">


    <meta name="enabled-features" content="MARKETPLACE_FEATURED_BLOG_POSTS,MARKETPLACE_INVOICED_BILLING,MARKETPLACE_SOCIAL_PROOF_CUSTOMERS,MARKETPLACE_TRENDING_SOCIAL_PROOF,MARKETPLACE_RECOMMENDATIONS,MARKETPLACE_PENDING_INSTALLATIONS,RELATED_ISSUES">

  <meta http-equiv="x-pjax-version" content="ba65740e1945c031031522a2bd89072b">
  

      <link href="https://github.com/hjzCy/sql_node/commits/master.atom" rel="alternate" title="Recent Commits to sql_node:master" type="application/atom+xml">

  <meta name="go-import" content="github.com/hjzCy/sql_node git https://github.com/hjzCy/sql_node.git">

  <meta name="octolytics-dimension-user_id" content="39392770" /><meta name="octolytics-dimension-user_login" content="hjzCy" /><meta name="octolytics-dimension-repository_id" content="199999481" /><meta name="octolytics-dimension-repository_nwo" content="hjzCy/sql_node" /><meta name="octolytics-dimension-repository_public" content="true" /><meta name="octolytics-dimension-repository_is_fork" content="false" /><meta name="octolytics-dimension-repository_network_root_id" content="199999481" /><meta name="octolytics-dimension-repository_network_root_nwo" content="hjzCy/sql_node" /><meta name="octolytics-dimension-repository_explore_github_marketplace_ci_cta_shown" content="false" />


    <link rel="canonical" href="https://github.com/hjzCy/sql_node/blob/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md" data-pjax-transient>


  <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">

  <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">

  <link rel="mask-icon" href="https://github.githubassets.com/pinned-octocat.svg" color="#000000">
  <link rel="icon" type="image/x-icon" class="js-site-favicon" href="https://github.githubassets.com/favicon.ico">

<meta name="theme-color" content="#1e2327">


  <link rel="manifest" href="/manifest.json" crossOrigin="use-credentials">

  </head>

  <body class="logged-out env-production page-responsive page-blob">
    

  <div class="position-relative js-header-wrapper ">
    <a href="#start-of-content" class="px-2 py-4 bg-blue text-white show-on-focus js-skip-to-content">Skip to content</a>
    <span class="Progress progress-pjax-loader position-fixed width-full js-pjax-loader-bar">
      <span class="progress-pjax-loader-bar top-0 left-0" style="width: 0%;"></span>
    </span>

    
    



        <header class="Header-old header-logged-out js-details-container Details position-relative f4 py-2" role="banner">
  <div class="container-lg d-lg-flex flex-items-center p-responsive">
    <div class="d-flex flex-justify-between flex-items-center">
        <a class="mr-4" href="https://github.com/" aria-label="Homepage" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
          <svg height="32" class="octicon octicon-mark-github text-white" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"/></svg>
        </a>

          <div class="d-lg-none css-truncate css-truncate-target width-fit p-2">
            
              <svg class="octicon octicon-repo" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
    <a class="Header-link" href="/hjzCy">hjzCy</a>
    /
    <a class="Header-link" href="/hjzCy/sql_node">sql_node</a>


          </div>

        <div class="d-flex flex-items-center">
            <a href="/join?source=header-repo"
              class="d-inline-block d-lg-none f5 text-white no-underline border border-gray-dark rounded-2 px-2 py-1 mr-3 mr-sm-5"
              data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;site header&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;SIGN_UP&quot;,&quot;originating_url&quot;:&quot;https://github.com/hjzCy/sql_node/blob/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md&quot;,&quot;user_id&quot;:null}}" data-hydro-click-hmac="3412a9ed904435bbb207adfe84473cab21e2d23c99929d22e89120ef21da8ac1"
              data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">
              Sign&nbsp;up
            </a>

          <button class="btn-link d-lg-none mt-1 js-details-target" type="button" aria-label="Toggle navigation" aria-expanded="false">
            <svg height="24" class="octicon octicon-three-bars text-white" viewBox="0 0 12 16" version="1.1" width="18" aria-hidden="true"><path fill-rule="evenodd" d="M11.41 9H.59C0 9 0 8.59 0 8c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zm0-4H.59C0 5 0 4.59 0 4c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zM.59 11H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1H.59C0 13 0 12.59 0 12c0-.59 0-1 .59-1z"/></svg>
          </button>
        </div>
    </div>

    <div class="HeaderMenu HeaderMenu--logged-out position-fixed top-0 right-0 bottom-0 height-fit position-lg-relative d-lg-flex flex-justify-between flex-items-center flex-auto">
      <div class="d-flex d-lg-none flex-justify-end border-bottom bg-gray-light p-3">
        <button class="btn-link js-details-target" type="button" aria-label="Toggle navigation" aria-expanded="false">
          <svg height="24" class="octicon octicon-x text-gray" viewBox="0 0 12 16" version="1.1" width="18" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
        </button>
      </div>

        <nav class="mt-0 px-3 px-lg-0 mb-5 mb-lg-0" aria-label="Global">
          <ul class="d-lg-flex list-style-none">
              <li class="d-block d-lg-flex flex-lg-nowrap flex-lg-items-center border-bottom border-lg-bottom-0 mr-0 mr-lg-3 edge-item-fix position-relative flex-wrap flex-justify-between d-flex flex-items-center ">
                <details class="HeaderMenu-details details-overlay details-reset width-full">
                  <summary class="HeaderMenu-summary HeaderMenu-link px-0 py-3 border-0 no-wrap d-block d-lg-inline-block">
                    Why GitHub?
                    <svg x="0px" y="0px" viewBox="0 0 14 8" xml:space="preserve" fill="none" class="icon-chevon-down-mktg position-absolute position-lg-relative">
                      <path d="M1,1l6.2,6L13,1"></path>
                    </svg>
                  </summary>
                  <div class="dropdown-menu flex-auto rounded-1 bg-white px-0 mt-0 pb-4 p-lg-4 position-relative position-lg-absolute left-0 left-lg-n4">
                    <a href="/features" class="py-2 lh-condensed-ultra d-block link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Features">Features <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a>
                    <ul class="list-style-none f5 pb-3">
                      <li class="edge-item-fix"><a href="/features/code-review/" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Code review">Code review</a></li>
                      <li class="edge-item-fix"><a href="/features/project-management/" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Project management">Project management</a></li>
                      <li class="edge-item-fix"><a href="/features/integrations" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Integrations">Integrations</a></li>
                      <li class="edge-item-fix"><a href="/features/actions" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Actions">Actions</a></li>
                          <li class="edge-item-fix"><a href="/features/packages" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to GitHub Packages">Packages</a></li>
                      <li class="edge-item-fix"><a href="/features/security" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Security">Security</a></li>
                      <li class="edge-item-fix"><a href="/features#team-management" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Team management">Team management</a></li>
                      <li class="edge-item-fix"><a href="/features#hosting" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Code hosting">Hosting</a></li>
                    </ul>

                    <ul class="list-style-none mb-0 border-lg-top pt-lg-3">
                      <li class="edge-item-fix"><a href="/customer-stories" class="py-2 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Customer stories">Customer stories <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                      <li class="edge-item-fix"><a href="/security" class="py-2 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Security">Security <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                    </ul>
                  </div>
                </details>
              </li>
              <li class="border-bottom border-lg-bottom-0 mr-0 mr-lg-3">
                <a href="/enterprise" class="HeaderMenu-link no-underline py-3 d-block d-lg-inline-block" data-ga-click="(Logged out) Header, go to Enterprise">Enterprise</a>
              </li>

              <li class="d-block d-lg-flex flex-lg-nowrap flex-lg-items-center border-bottom border-lg-bottom-0 mr-0 mr-lg-3 edge-item-fix position-relative flex-wrap flex-justify-between d-flex flex-items-center ">
                <details class="HeaderMenu-details details-overlay details-reset width-full">
                  <summary class="HeaderMenu-summary HeaderMenu-link px-0 py-3 border-0 no-wrap d-block d-lg-inline-block">
                    Explore
                    <svg x="0px" y="0px" viewBox="0 0 14 8" xml:space="preserve" fill="none" class="icon-chevon-down-mktg position-absolute position-lg-relative">
                      <path d="M1,1l6.2,6L13,1"></path>
                    </svg>
                  </summary>

                  <div class="dropdown-menu flex-auto rounded-1 bg-white px-0 pt-2 pb-0 mt-0 pb-4 p-lg-4 position-relative position-lg-absolute left-0 left-lg-n4">
                    <ul class="list-style-none mb-3">
                      <li class="edge-item-fix"><a href="/explore" class="py-2 lh-condensed-ultra d-block link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Explore">Explore GitHub <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                    </ul>

                    <h4 class="text-gray-light text-normal text-mono f5 mb-2 border-lg-top pt-lg-3">Learn &amp; contribute</h4>
                    <ul class="list-style-none mb-3">
                      <li class="edge-item-fix"><a href="/topics" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Topics">Topics</a></li>
                        <li class="edge-item-fix"><a href="/collections" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Collections">Collections</a></li>
                      <li class="edge-item-fix"><a href="/trending" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Trending">Trending</a></li>
                      <li class="edge-item-fix"><a href="https://lab.github.com/" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Learning lab">Learning Lab</a></li>
                      <li class="edge-item-fix"><a href="https://opensource.guide" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Open source guides">Open source guides</a></li>
                    </ul>

                    <h4 class="text-gray-light text-normal text-mono f5 mb-2 border-lg-top pt-lg-3">Connect with others</h4>
                    <ul class="list-style-none mb-0">
                      <li class="edge-item-fix"><a href="https://github.com/events" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Events">Events</a></li>
                      <li class="edge-item-fix"><a href="https://github.community" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Community forum">Community forum</a></li>
                      <li class="edge-item-fix"><a href="https://education.github.com" class="py-2 pb-0 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to GitHub Education">GitHub Education</a></li>
                    </ul>
                  </div>
                </details>
              </li>

              <li class="border-bottom border-lg-bottom-0 mr-0 mr-lg-3">
                <a href="/marketplace" class="HeaderMenu-link no-underline py-3 d-block d-lg-inline-block" data-ga-click="(Logged out) Header, go to Marketplace">Marketplace</a>
              </li>

              <li class="d-block d-lg-flex flex-lg-nowrap flex-lg-items-center border-bottom border-lg-bottom-0 mr-0 mr-lg-3 edge-item-fix position-relative flex-wrap flex-justify-between d-flex flex-items-center ">
                <details class="HeaderMenu-details details-overlay details-reset width-full">
                  <summary class="HeaderMenu-summary HeaderMenu-link px-0 py-3 border-0 no-wrap d-block d-lg-inline-block">
                    Pricing
                    <svg x="0px" y="0px" viewBox="0 0 14 8" xml:space="preserve" fill="none" class="icon-chevon-down-mktg position-absolute position-lg-relative">
                       <path d="M1,1l6.2,6L13,1"></path>
                    </svg>
                  </summary>

                  <div class="dropdown-menu flex-auto rounded-1 bg-white px-0 pt-2 pb-4 mt-0 p-lg-4 position-relative position-lg-absolute left-0 left-lg-n4">
                    <a href="/pricing" class="pb-2 lh-condensed-ultra d-block link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Pricing">Plans <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a>

                    <ul class="list-style-none mb-3">
                      <li class="edge-item-fix"><a href="/pricing#feature-comparison" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Compare plans">Compare plans</a></li>
                      <li class="edge-item-fix"><a href="https://enterprise.github.com/contact" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Contact Sales">Contact Sales</a></li>
                    </ul>

                    <ul class="list-style-none mb-0 border-lg-top pt-lg-3">
                      <li class="edge-item-fix"><a href="/nonprofit" class="py-2 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Nonprofits">Nonprofit <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                      <li class="edge-item-fix"><a href="https://education.github.com" class="py-2 pb-0 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover"  data-ga-click="(Logged out) Header, go to Education">Education <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                    </ul>
                  </div>
                </details>
              </li>
          </ul>
        </nav>

      <div class="d-lg-flex flex-items-center px-3 px-lg-0 text-center text-lg-left">
          <div class="d-lg-flex mb-3 mb-lg-0">
            <div class="header-search flex-self-stretch flex-lg-self-auto mr-0 mr-lg-3 mb-3 mb-lg-0 scoped-search site-scoped-search js-site-search position-relative js-jump-to"
  role="combobox"
  aria-owns="jump-to-results"
  aria-label="Search or jump to"
  aria-haspopup="listbox"
  aria-expanded="false"
>
  <div class="position-relative">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-site-search-form" role="search" aria-label="Site" data-scope-type="Repository" data-scope-id="199999481" data-scoped-search-url="/hjzCy/sql_node/search" data-unscoped-search-url="/search" action="/hjzCy/sql_node/search" accept-charset="UTF-8" method="get">
      <label class="form-control input-sm header-search-wrapper p-0 header-search-wrapper-jump-to position-relative d-flex flex-justify-between flex-items-center js-chromeless-input-container">
        <input type="text"
          class="form-control input-sm header-search-input jump-to-field js-jump-to-field js-site-search-focus js-site-search-field is-clearable"
          data-hotkey="s,/"
          name="q"
          value=""
          placeholder="Search"
          data-unscoped-placeholder="Search GitHub"
          data-scoped-placeholder="Search"
          autocapitalize="off"
          aria-autocomplete="list"
          aria-controls="jump-to-results"
          aria-label="Search"
          data-jump-to-suggestions-path="/_graphql/GetSuggestedNavigationDestinations"
          spellcheck="false"
          autocomplete="off"
          >
          <input type="hidden" data-csrf="true" class="js-data-jump-to-suggestions-path-csrf" value="RimdbSTZVNDcSnwG+66UijUad4hf7py+adbknB6PWX18BXbwMygDlbxBOFL7gSVDPmu+trjByXPtW0cda4DkCA==" />
          <input type="hidden" class="js-site-search-type-field" name="type" >
            <img src="https://github.githubassets.com/images/search-key-slash.svg" alt="" class="mr-2 header-search-key-slash">

            <div class="Box position-absolute overflow-hidden d-none jump-to-suggestions js-jump-to-suggestions-container">
              
<ul class="d-none js-jump-to-suggestions-template-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-suggestion" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 00-1 1v14a1 1 0 001 1h13a1 1 0 001-1V1a1 1 0 00-1-1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0013 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 000-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>

</ul>

<ul class="d-none js-jump-to-no-results-template-container">
  <li class="d-flex flex-justify-center flex-items-center f5 d-none js-jump-to-suggestion p-2">
    <span class="text-gray">No suggested jump to results</span>
  </li>
</ul>

<ul id="jump-to-results" role="listbox" class="p-0 m-0 js-navigation-container jump-to-suggestions-results-container js-jump-to-suggestions-results-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-scoped-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 00-1 1v14a1 1 0 001 1h13a1 1 0 001-1V1a1 1 0 00-1-1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0013 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 000-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>

  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-global-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 00-1 1v14a1 1 0 001 1h13a1 1 0 001-1V1a1 1 0 00-1-1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0013 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 000-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>


</ul>

            </div>
      </label>
</form>  </div>
</div>

          </div>

        <a href="/login?return_to=%2FhjzCy%2Fsql_node%2Fblob%2Fmaster%2Fmysql%2FMySQL%25E5%25AD%25A6%25E4%25B9%25A0%25E7%25AC%2594%25E8%25AE%25B0.md"
          class="HeaderMenu-link no-underline mr-3"
          data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;site header menu&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;SIGN_UP&quot;,&quot;originating_url&quot;:&quot;https://github.com/hjzCy/sql_node/blob/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md&quot;,&quot;user_id&quot;:null}}" data-hydro-click-hmac="fe4bf84a752739c4bbcfdde2f197fb50568ac1f477aa3835755625b926d06ac2"
          data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">
          Sign&nbsp;in
        </a>
          <a href="/join?source=header-repo&amp;source_repo=hjzCy%2Fsql_node"
            class="HeaderMenu-link d-inline-block no-underline border border-gray-dark rounded-1 px-2 py-1"
            data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;site header menu&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;SIGN_UP&quot;,&quot;originating_url&quot;:&quot;https://github.com/hjzCy/sql_node/blob/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md&quot;,&quot;user_id&quot;:null}}" data-hydro-click-hmac="fe4bf84a752739c4bbcfdde2f197fb50568ac1f477aa3835755625b926d06ac2"
            data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">
            Sign&nbsp;up
          </a>
      </div>
    </div>
  </div>
</header>

  </div>

  <div id="start-of-content" class="show-on-focus"></div>


    <div id="js-flash-container">

</div>


      

  <include-fragment class="js-notification-shelf-include-fragment" data-base-src="https://github.com/notifications/beta/shelf"></include-fragment>




  <div class="application-main " data-commit-hovercards-enabled>
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode" class="">
    <main  >
      

  











  <div class="pagehead repohead hx_repohead readability-menu bg-gray-light pb-0 pt-0 pt-lg-3">

    <div class="d-flex container-lg mb-4 p-responsive d-none d-lg-flex">

      <div class="flex-auto min-width-0 width-fit mr-3">
        <h1 class="public  d-flex flex-wrap flex-items-center break-word float-none ">
    <svg class="octicon octicon-repo" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
  <span class="author ml-1 flex-self-stretch" itemprop="author">
    <a class="url fn" rel="author" data-hovercard-type="user" data-hovercard-url="/users/hjzCy/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/hjzCy">hjzCy</a>
  </span>
  <span class="path-divider flex-self-stretch">/</span>
  <strong itemprop="name" class="mr-2 flex-self-stretch">
    <a data-pjax="#js-repo-pjax-container" href="/hjzCy/sql_node">sql_node</a>
  </strong>
  
</h1>


      </div>

      <ul class="pagehead-actions flex-shrink-0 " >




  <li>
    
  <a class="tooltipped tooltipped-s btn btn-sm btn-with-count" aria-label="You must be signed in to watch a repository" rel="nofollow" data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;notification subscription menu watch&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;LOG_IN&quot;,&quot;originating_url&quot;:&quot;https://github.com/hjzCy/sql_node/blob/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md&quot;,&quot;user_id&quot;:null}}" data-hydro-click-hmac="e8272a72c647893765f8724f7222d55ef3e96c70510bfddb4b06d3c61be1e035" href="/login?return_to=%2FhjzCy%2Fsql_node">
    <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
    Watch
</a>    <a class="social-count" href="/hjzCy/sql_node/watchers"
       aria-label="1 user is watching this repository">
      1
    </a>

  </li>

  <li>
        <a class="btn btn-sm btn-with-count tooltipped tooltipped-s" aria-label="You must be signed in to star a repository" rel="nofollow" data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;star button&quot;,&quot;repository_id&quot;:199999481,&quot;auth_type&quot;:&quot;LOG_IN&quot;,&quot;originating_url&quot;:&quot;https://github.com/hjzCy/sql_node/blob/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md&quot;,&quot;user_id&quot;:null}}" data-hydro-click-hmac="35be1077c7c41629bd7bbcadb261421fb76041cffa01479907ae571d66d6fc59" href="/login?return_to=%2FhjzCy%2Fsql_node">
      <svg height="16" class="octicon octicon-star v-align-text-bottom" vertical_align="text_bottom" viewBox="0 0 14 16" version="1.1" width="14" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"/></svg>

      Star
</a>
    <a class="social-count js-social-count" href="/hjzCy/sql_node/stargazers"
      aria-label="106 users starred this repository">
      106
    </a>

  </li>

  <li>
      <a class="btn btn-sm btn-with-count tooltipped tooltipped-s" aria-label="You must be signed in to fork a repository" rel="nofollow" data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;repo details fork button&quot;,&quot;repository_id&quot;:199999481,&quot;auth_type&quot;:&quot;LOG_IN&quot;,&quot;originating_url&quot;:&quot;https://github.com/hjzCy/sql_node/blob/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md&quot;,&quot;user_id&quot;:null}}" data-hydro-click-hmac="06e54b775ef88ab6e5c7d4674358e437689fa051bb492c20dd4b5a2b5c721b23" href="/login?return_to=%2FhjzCy%2Fsql_node">
        <svg class="octicon octicon-repo-forked v-align-text-bottom" viewBox="0 0 10 16" version="1.1" width="10" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 1a1.993 1.993 0 00-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 002 1a1.993 1.993 0 00-1 3.72V6.5l3 3v1.78A1.993 1.993 0 005 15a1.993 1.993 0 001-3.72V9.5l3-3V4.72A1.993 1.993 0 008 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
        Fork
</a>
    <a href="/hjzCy/sql_node/network/members" class="social-count"
       aria-label="164 users forked this repository">
      164
    </a>
  </li>
</ul>

    </div>
      
<nav class="hx_reponav reponav js-repo-nav js-sidenav-container-pjax clearfix container-lg p-responsive d-none d-lg-block"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
    aria-label="Repository"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a class="js-selected-navigation-item selected reponav-item" itemprop="url" data-hotkey="g c" aria-current="page" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages /hjzCy/sql_node" href="/hjzCy/sql_node">
      <div class="d-inline"><svg class="octicon octicon-code" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"/></svg></div>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a itemprop="url" data-hotkey="g i" class="js-selected-navigation-item reponav-item" data-selected-links="repo_issues repo_labels repo_milestones /hjzCy/sql_node/issues" href="/hjzCy/sql_node/issues">
        <div class="d-inline"><svg class="octicon octicon-issue-opened" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 011.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"/></svg></div>
        <span itemprop="name">Issues</span>
        <span class="Counter">0</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a data-hotkey="g p" data-skip-pjax="true" itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_pulls checks /hjzCy/sql_node/pulls" href="/hjzCy/sql_node/pulls">
      <div class="d-inline"><svg class="octicon octicon-git-pull-request" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0010 15a1.993 1.993 0 001-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 00-1 3.72v6.56A1.993 1.993 0 002 15a1.993 1.993 0 001-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg></div>
      <span itemprop="name">Pull requests</span>
      <span class="Counter">0</span>
      <meta itemprop="position" content="4">
</a>  </span>


    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement" class="position-relative float-left">
      <a data-hotkey="g w" data-skip-pjax="true" class="js-selected-navigation-item reponav-item" data-selected-links="repo_actions /hjzCy/sql_node/actions" href="/hjzCy/sql_node/actions">
        <div class="d-inline"><svg class="octicon octicon-play" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 8A7 7 0 110 8a7 7 0 0114 0zm-8.223 3.482l4.599-3.066a.5.5 0 000-.832L5.777 4.518A.5.5 0 005 4.934v6.132a.5.5 0 00.777.416z"/></svg></div>
        Actions
</a>
    </span>

    <a data-hotkey="g b" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /hjzCy/sql_node/projects" href="/hjzCy/sql_node/projects">
      <div class="d-inline"><svg class="octicon octicon-project" viewBox="0 0 15 16" version="1.1" width="15" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 00-1 1v14a1 1 0 001 1h13a1 1 0 001-1V1a1 1 0 00-1-1z"/></svg></div>
      Projects
      <span class="Counter">0</span>
</a>

    <a data-skip-pjax="true" class="js-selected-navigation-item reponav-item" data-selected-links="security alerts policy token_scanning code_scanning /hjzCy/sql_node/security/advisories" href="/hjzCy/sql_node/security/advisories">
      <div class="d-inline"><svg class="octicon octicon-shield" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 2l7-2 7 2v6.02C14 12.69 8.69 16 7 16c-1.69 0-7-3.31-7-7.98V2zm1 .75L7 1l6 1.75v5.268C13 12.104 8.449 15 7 15c-1.449 0-6-2.896-6-6.982V2.75zm1 .75L7 2v12c-1.207 0-5-2.482-5-5.985V3.5z"/></svg></div>
      Security
</a>
    <a class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors dependency_graph pulse people /hjzCy/sql_node/pulse" href="/hjzCy/sql_node/pulse">
      <div class="d-inline"><svg class="octicon octicon-graph" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"/></svg></div>
      Insights
</a>

</nav>

  <div class="reponav-wrapper reponav-small d-lg-none">
  <nav class="reponav js-reponav text-center no-wrap"
       itemscope
       itemtype="http://schema.org/BreadcrumbList">

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a class="js-selected-navigation-item selected reponav-item" itemprop="url" aria-current="page" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages /hjzCy/sql_node" href="/hjzCy/sql_node">
        <span itemprop="name">Code</span>
        <meta itemprop="position" content="1">
</a>    </span>

      <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
        <a itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_issues repo_labels repo_milestones /hjzCy/sql_node/issues" href="/hjzCy/sql_node/issues">
          <span itemprop="name">Issues</span>
          <span class="Counter">0</span>
          <meta itemprop="position" content="2">
</a>      </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_pulls checks /hjzCy/sql_node/pulls" href="/hjzCy/sql_node/pulls">
        <span itemprop="name">Pull requests</span>
        <span class="Counter">0</span>
        <meta itemprop="position" content="4">
</a>    </span>


      <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
        <a itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /hjzCy/sql_node/projects" href="/hjzCy/sql_node/projects">
          <span itemprop="name">Projects</span>
          <span class="Counter">0</span>
          <meta itemprop="position" content="5">
</a>      </span>

      <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
        <a itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_actions /hjzCy/sql_node/actions" href="/hjzCy/sql_node/actions">
          <span itemprop="name">Actions</span>
          <meta itemprop="position" content="6">
</a>      </span>


      <a itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="security alerts policy token_scanning code_scanning /hjzCy/sql_node/security/advisories" href="/hjzCy/sql_node/security/advisories">
        <span itemprop="name">Security</span>
        <meta itemprop="position" content="8">
</a>
      <a class="js-selected-navigation-item reponav-item" data-selected-links="pulse /hjzCy/sql_node/pulse" href="/hjzCy/sql_node/pulse">
        Pulse
</a>

  </nav>
</div>


  </div>

  

  <include-fragment class="js-notification-shelf-include-fragment" data-base-src="https://github.com/notifications/beta/shelf"></include-fragment>


<div class="container-lg clearfix new-discussion-timeline  p-responsive">
  <div class="repository-content ">

    
    


  


    <a class="d-none js-permalink-shortcut" data-hotkey="y" href="/hjzCy/sql_node/blob/dd9913ea7bd76d522ea6284b5dd7b1c5a47b552b/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md">Permalink</a>

    <!-- blob contrib key: blob_contributors:v22:987b193907215f1f99c4a064a6f5707b -->
      <div class="signup-prompt-bg rounded-1 js-signup-prompt" data-prompt="signup" hidden>
    <div class="signup-prompt p-4 text-center mb-4 rounded-1">
      <div class="position-relative">
        <button type="button" class="position-absolute top-0 right-0 btn-link link-gray js-signup-prompt-button" data-ga-click="(Logged out) Sign up prompt, clicked Dismiss, text:dismiss">
          Dismiss
        </button>
        <h3 class="pt-2">Join GitHub today</h3>
        <p class="col-6 mx-auto">GitHub is home to over 40 million developers working together to host and review code, manage projects, and build software together.</p>
        <a class="btn btn-primary" data-ga-click="(Logged out) Sign up prompt, clicked Sign up, text:sign-up" data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;files signup prompt&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;SIGN_UP&quot;,&quot;originating_url&quot;:&quot;https://github.com/hjzCy/sql_node/blob/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md&quot;,&quot;user_id&quot;:null}}" data-hydro-click-hmac="44e3bf0e310da77346fd2462e9a66df42861505fc99e0f46d4635e00b09768c1" href="/join?source=prompt-blob-show&amp;source_repo=hjzCy%2Fsql_node">Sign up</a>
      </div>
    </div>
  </div>


    <div class="d-flex flex-items-start flex-shrink-0 flex-column flex-md-row pb-3">
      <span class="d-flex flex-justify-between width-full width-md-auto">
        
<details class="details-reset details-overlay branch-select-menu " id="branch-select-menu">
  <summary class="btn btn-sm css-truncate"
           data-hotkey="w"
           title="Switch branches or tags">
    <i>Branch:</i>
    <span class="css-truncate-target" data-menu-button>master</span>
    <span class="dropdown-caret"></span>
  </summary>

  <details-menu class="SelectMenu SelectMenu--hasFilter" src="/hjzCy/sql_node/refs/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md?source_action=show&amp;source_controller=blob" preload>
    <div class="SelectMenu-modal">
      <include-fragment class="SelectMenu-loading" aria-label="Menu is loading">
        <svg class="octicon octicon-octoface anim-pulse" height="32" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M14.7 5.34c.13-.32.55-1.59-.13-3.31 0 0-1.05-.33-3.44 1.3-1-.28-2.07-.32-3.13-.32s-2.13.04-3.13.32c-2.39-1.64-3.44-1.3-3.44-1.3-.68 1.72-.26 2.99-.13 3.31C.49 6.21 0 7.33 0 8.69 0 13.84 3.33 15 7.98 15S16 13.84 16 8.69c0-1.36-.49-2.48-1.3-3.35zM8 14.02c-3.3 0-5.98-.15-5.98-3.35 0-.76.38-1.48 1.02-2.07 1.07-.98 2.9-.46 4.96-.46 2.07 0 3.88-.52 4.96.46.65.59 1.02 1.3 1.02 2.07 0 3.19-2.68 3.35-5.98 3.35zM5.49 9.01c-.66 0-1.2.8-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.54-1.78-1.2-1.78zm5.02 0c-.66 0-1.2.79-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.53-1.78-1.2-1.78z"/></svg>
      </include-fragment>
    </div>
  </details-menu>
</details>

        <div class="BtnGroup flex-shrink-0 d-md-none">
          <a href="/hjzCy/sql_node/find/master"
                class="js-pjax-capture-input btn btn-sm BtnGroup-item"
                data-pjax
                data-hotkey="t">
            Find file
          </a>
          <clipboard-copy value="mysql/MySQL学习笔记.md" class="btn btn-sm BtnGroup-item">
            Copy path
          </clipboard-copy>
        </div>
      </span>
      <h2 id="blob-path" class="breadcrumb flex-auto min-width-0 text-normal flex-md-self-center ml-md-2 mr-md-3 my-2 my-md-0">
        <span class="js-repo-root text-bold"><span class="js-path-segment"><a data-pjax="true" href="/hjzCy/sql_node"><span>sql_node</span></a></span></span><span class="separator">/</span><span class="js-path-segment"><a data-pjax="true" href="/hjzCy/sql_node/tree/master/mysql"><span>mysql</span></a></span><span class="separator">/</span><strong class="final-path">MySQL学习笔记.md</strong>
      </h2>

      <div class="BtnGroup flex-shrink-0 d-none d-md-inline-block">
        <a href="/hjzCy/sql_node/find/master"
              class="js-pjax-capture-input btn btn-sm BtnGroup-item"
              data-pjax
              data-hotkey="t">
          Find file
        </a>
        <clipboard-copy value="mysql/MySQL学习笔记.md" class="btn btn-sm BtnGroup-item">
          Copy path
        </clipboard-copy>
      </div>
    </div>

    



    
  <div class="Box Box--condensed d-flex flex-column flex-shrink-0">
      <div class="Box-body d-flex flex-justify-between bg-blue-light flex-column flex-md-row flex-items-start flex-md-items-center">
        <span class="pr-md-4 f6">
          <a rel="author" data-skip-pjax="true" data-hovercard-type="user" data-hovercard-url="/users/hjzCy/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/hjzCy"><img class="avatar" src="https://avatars1.githubusercontent.com/u/39392770?s=40&amp;v=4" width="20" height="20" alt="@hjzCy" /></a>
          <a class="text-bold link-gray-dark lh-default v-align-middle" rel="author" data-hovercard-type="user" data-hovercard-url="/users/hjzCy/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/hjzCy">hjzCy</a>
            <span class="lh-default v-align-middle">
              <a data-pjax="true" title="Update MySQL学习笔记.md" class="link-gray" href="/hjzCy/sql_node/commit/dd9913ea7bd76d522ea6284b5dd7b1c5a47b552b">Update MySQL学习笔记.md</a>
            </span>
        </span>
        <span class="d-inline-block flex-shrink-0 v-align-bottom f6 mt-2 mt-md-0">
          <a class="pr-2 text-mono link-gray" href="/hjzCy/sql_node/commit/dd9913ea7bd76d522ea6284b5dd7b1c5a47b552b" data-pjax>dd9913e</a>
          <relative-time datetime="2019-08-06T12:22:27Z" class="no-wrap">Aug 6, 2019</relative-time>
        </span>
      </div>

    <div class="Box-body d-flex flex-items-center flex-auto f6 border-bottom-0 flex-wrap" >
      <details class="details-reset details-overlay details-overlay-dark lh-default text-gray-dark float-left mr-2" id="blob_contributors_box">
        <summary class="btn-link">
          <span><strong>1</strong> contributor</span>
        </summary>
        <details-dialog
          class="Box Box--overlay d-flex flex-column anim-fade-in fast"
          aria-label="Users who have contributed to this file"
          src="/hjzCy/sql_node/contributors-list/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md" preload>
          <div class="Box-header">
            <button class="Box-btn-octicon btn-octicon float-right" type="button" aria-label="Close dialog" data-close-dialog>
              <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
            </button>
            <h3 class="Box-title">
              Users who have contributed to this file
            </h3>
          </div>
          <include-fragment class="octocat-spinner my-3" aria-label="Loading..."></include-fragment>
        </details-dialog>
      </details>
    </div>
  </div>






    <div class="Box mt-3 position-relative
      ">
      
<div class="Box-header py-2 d-flex flex-column flex-shrink-0 flex-md-row flex-md-items-center">
  <div class="text-mono f6 flex-auto pr-3 flex-order-2 flex-md-order-1 mt-2 mt-md-0">

      1974 lines (1606 sloc)
      <span class="file-info-divider"></span>
    54.5 KB
  </div>

  <div class="d-flex py-1 py-md-0 flex-auto flex-order-1 flex-md-order-2 flex-sm-grow-0 flex-justify-between">

    <div class="BtnGroup">
      <a id="raw-url" class="btn btn-sm BtnGroup-item" href="/hjzCy/sql_node/raw/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md">Raw</a>
        <a class="btn btn-sm js-update-url-with-hash BtnGroup-item" data-hotkey="b" href="/hjzCy/sql_node/blame/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md">Blame</a>
      <a rel="nofollow" class="btn btn-sm BtnGroup-item" href="/hjzCy/sql_node/commits/master/mysql/MySQL%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.md">History</a>
    </div>


    <div>
          <a class="btn-octicon tooltipped tooltipped-nw js-remove-unless-platform"
             data-platforms="windows,mac"
             href="https://desktop.github.com"
             aria-label="Open this file in GitHub Desktop"
             data-ga-click="Repository, open with desktop">
              <svg class="octicon octicon-device-desktop" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M15 2H1c-.55 0-1 .45-1 1v9c0 .55.45 1 1 1h5.34c-.25.61-.86 1.39-2.34 2h8c-1.48-.61-2.09-1.39-2.34-2H15c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm0 9H1V3h14v8z"/></svg>
          </a>

          <button type="button" class="btn-octicon disabled tooltipped tooltipped-nw"
            aria-label="You must be signed in to make or propose changes">
            <svg class="octicon octicon-pencil" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 011.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"/></svg>
          </button>
          <button type="button" class="btn-octicon btn-octicon-danger disabled tooltipped tooltipped-nw"
            aria-label="You must be signed in to make or propose changes">
            <svg class="octicon octicon-trashcan" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"/></svg>
          </button>
    </div>
  </div>
</div>




      
  <div id="readme" class="Box-body readme blob js-code-block-container">
    <article class="markdown-body entry-content p-3 p-md-6" itemprop="text"><h1><a id="user-content-mysql学习笔记" class="anchor" aria-hidden="true" href="#mysql学习笔记"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>MySQL学习笔记</h1>
<h2><a id="user-content-登录和退出mysql服务器" class="anchor" aria-hidden="true" href="#登录和退出mysql服务器"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>登录和退出MySQL服务器</h2>
<div class="highlight highlight-source-shell"><pre><span class="pl-c"><span class="pl-c">#</span> 登录MySQL</span>
$ mysql -u root -p12345612

<span class="pl-c"><span class="pl-c">#</span> 退出MySQL数据库服务器</span>
<span class="pl-c1">exit</span><span class="pl-k">;</span></pre></div>
<h2><a id="user-content-基本语法" class="anchor" aria-hidden="true" href="#基本语法"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>基本语法</h2>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 显示所有数据库</span>
show databases;

<span class="pl-c"><span class="pl-c">--</span> 创建数据库</span>
<span class="pl-k">CREATE</span> <span class="pl-k">DATABASE</span> <span class="pl-en">test</span>;

<span class="pl-c"><span class="pl-c">--</span> 切换数据库</span>
use test;

<span class="pl-c"><span class="pl-c">--</span> 显示数据库中的所有表</span>
show tables;

<span class="pl-c"><span class="pl-c">--</span> 创建数据表</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">pet</span> (
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    owner <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    species <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    sex <span class="pl-k">CHAR</span>(<span class="pl-c1">1</span>),
    birth <span class="pl-k">DATE</span>,
    death <span class="pl-k">DATE</span>
);

<span class="pl-c"><span class="pl-c">--</span> 查看数据表结构</span>
<span class="pl-c"><span class="pl-c">--</span> describe pet;</span>
<span class="pl-k">desc</span> pet;

<span class="pl-c"><span class="pl-c">--</span> 查询表</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">from</span> pet;

<span class="pl-c"><span class="pl-c">--</span> 插入数据</span>
<span class="pl-k">INSERT INTO</span> pet <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>puffball<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Diane<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>hamster<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>f<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1990-03-30<span class="pl-pds">'</span></span>, <span class="pl-k">NULL</span>);

<span class="pl-c"><span class="pl-c">--</span> 修改数据</span>
<span class="pl-k">UPDATE</span> pet <span class="pl-k">SET</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>squirrel<span class="pl-pds">'</span></span> <span class="pl-k">where</span> owner <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>Diane<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> 删除数据</span>
<span class="pl-k">DELETE</span> <span class="pl-k">FROM</span> pet <span class="pl-k">where</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>squirrel<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> 删除表</span>
<span class="pl-k">DROP</span> <span class="pl-k">TABLE</span> myorder;</pre></div>
<h2><a id="user-content-建表约束" class="anchor" aria-hidden="true" href="#建表约束"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>建表约束</h2>
<h3><a id="user-content-主键约束" class="anchor" aria-hidden="true" href="#主键约束"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>主键约束</h3>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 主键约束</span>
<span class="pl-c"><span class="pl-c">--</span> 使某个字段不重复且不得为空，确保表内所有数据的唯一性。</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">user</span> (
    id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>)
);

<span class="pl-c"><span class="pl-c">--</span> 联合主键</span>
<span class="pl-c"><span class="pl-c">--</span> 联合主键中的每个字段都不能为空，并且加起来不能和已设置的联合主键重复。</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">user</span> (
    id <span class="pl-k">INT</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    password <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    <span class="pl-k">PRIMARY KEY</span>(id, name)
);

<span class="pl-c"><span class="pl-c">--</span> 自增约束</span>
<span class="pl-c"><span class="pl-c">--</span> 自增约束的主键由系统自动递增分配。</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">user</span> (
    id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span> AUTO_INCREMENT,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>)
);

<span class="pl-c"><span class="pl-c">--</span> 添加主键约束</span>
<span class="pl-c"><span class="pl-c">--</span> 如果忘记设置主键，还可以通过SQL语句设置（两种方式）：</span>
<span class="pl-k">ALTER</span> <span class="pl-k">TABLE</span> user ADD <span class="pl-k">PRIMARY KEY</span>(id);
<span class="pl-k">ALTER</span> <span class="pl-k">TABLE</span> user MODIFY id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>;

<span class="pl-c"><span class="pl-c">--</span> 删除主键</span>
<span class="pl-k">ALTER</span> <span class="pl-k">TABLE</span> user drop <span class="pl-k">PRIMARY KEY</span>;</pre></div>
<h3><a id="user-content-唯一主键" class="anchor" aria-hidden="true" href="#唯一主键"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>唯一主键</h3>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 建表时创建唯一主键</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">user</span> (
    id <span class="pl-k">INT</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    UNIQUE(name)
);

<span class="pl-c"><span class="pl-c">--</span> 添加唯一主键</span>
<span class="pl-c"><span class="pl-c">--</span> 如果建表时没有设置唯一建，还可以通过SQL语句设置（两种方式）：</span>
<span class="pl-k">ALTER</span> <span class="pl-k">TABLE</span> user ADD UNIQUE(name);
<span class="pl-k">ALTER</span> <span class="pl-k">TABLE</span> user MODIFY name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) UNIQUE;

<span class="pl-c"><span class="pl-c">--</span> 删除唯一主键</span>
<span class="pl-k">ALTER</span> <span class="pl-k">TABLE</span> user DROP INDEX name;</pre></div>
<h3><a id="user-content-非空约束" class="anchor" aria-hidden="true" href="#非空约束"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>非空约束</h3>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 建表时添加非空约束</span>
<span class="pl-c"><span class="pl-c">--</span> 约束某个字段不能为空</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">user</span> (
    id <span class="pl-k">INT</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">NOT NULL</span>
);

<span class="pl-c"><span class="pl-c">--</span> 移除非空约束</span>
<span class="pl-k">ALTER</span> <span class="pl-k">TABLE</span> user MODIFY name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>);</pre></div>
<h3><a id="user-content-默认约束" class="anchor" aria-hidden="true" href="#默认约束"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>默认约束</h3>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 建表时添加默认约束</span>
<span class="pl-c"><span class="pl-c">--</span> 约束某个字段的默认值</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">user2</span> (
    id <span class="pl-k">INT</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    age <span class="pl-k">INT</span> DEFAULT <span class="pl-c1">10</span>
);

<span class="pl-c"><span class="pl-c">--</span> 移除非空约束</span>
<span class="pl-k">ALTER</span> <span class="pl-k">TABLE</span> user MODIFY age <span class="pl-k">INT</span>;</pre></div>
<h3><a id="user-content-外键约束" class="anchor" aria-hidden="true" href="#外键约束"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>外键约束</h3>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 班级</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">classes</span> (
    id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>)
);

<span class="pl-c"><span class="pl-c">--</span> 学生表</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">students</span> (
    id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    <span class="pl-c"><span class="pl-c">--</span> 这里的 class_id 要和 classes 中的 id 字段相关联</span>
    class_id <span class="pl-k">INT</span>,
    <span class="pl-c"><span class="pl-c">--</span> 表示 class_id 的值必须来自于 classes 中的 id 字段值</span>
    <span class="pl-k">FOREIGN KEY</span>(class_id) <span class="pl-k">REFERENCES</span> classes(id)
);

<span class="pl-c"><span class="pl-c">--</span> 1. 主表（父表）classes 中没有的数据值，在副表（子表）students 中，是不可以使用的；</span>
<span class="pl-c"><span class="pl-c">--</span> 2. 主表中的记录被副表引用时，主表不可以被删除。</span></pre></div>
<h2><a id="user-content-数据库的三大设计范式" class="anchor" aria-hidden="true" href="#数据库的三大设计范式"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据库的三大设计范式</h2>
<h3><a id="user-content-1nf" class="anchor" aria-hidden="true" href="#1nf"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>1NF</h3>
<p>只要字段值还可以继续拆分，就不满足第一范式。</p>
<p>范式设计得越详细，对某些实际操作可能会更好，但并非都有好处，需要对项目的实际情况进行设定。</p>
<h3><a id="user-content-2nf" class="anchor" aria-hidden="true" href="#2nf"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>2NF</h3>
<p>在满足第一范式的前提下，其他列都必须完全依赖于主键列。如果出现不完全依赖，只可能发生在联合主键的情况下：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 订单表</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">myorder</span> (
    product_id <span class="pl-k">INT</span>,
    customer_id <span class="pl-k">INT</span>,
    product_name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    customer_name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    <span class="pl-k">PRIMARY KEY</span> (product_id, customer_id)
);</pre></div>
<p>实际上，在这张订单表中，<code>product_name</code> 只依赖于 <code>product_id</code> ，<code>customer_name</code> 只依赖于 <code>customer_id</code> 。也就是说，<code>product_name</code> 和 <code>customer_id</code> 是没用关系的，<code>customer_name</code> 和 <code>product_id</code> 也是没有关系的。</p>
<p>这就不满足第二范式：其他列都必须完全依赖于主键列！</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">myorder</span> (
    order_id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    product_id <span class="pl-k">INT</span>,
    customer_id <span class="pl-k">INT</span>
);

<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">product</span> (
    id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>)
);

<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">customer</span> (
    id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>)
);</pre></div>
<p>拆分之后，<code>myorder</code> 表中的 <code>product_id</code> 和 <code>customer_id</code> 完全依赖于 <code>order_id</code> 主键，而 <code>product</code> 和 <code>customer</code> 表中的其他字段又完全依赖于主键。满足了第二范式的设计！</p>
<h3><a id="user-content-3nf" class="anchor" aria-hidden="true" href="#3nf"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>3NF</h3>
<p>在满足第二范式的前提下，除了主键列之外，其他列之间不能有传递依赖关系。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">myorder</span> (
    order_id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    product_id <span class="pl-k">INT</span>,
    customer_id <span class="pl-k">INT</span>,
    customer_phone <span class="pl-k">VARCHAR</span>(<span class="pl-c1">15</span>)
);</pre></div>
<p>表中的 <code>customer_phone</code> 有可能依赖于 <code>order_id</code> 、 <code>customer_id</code> 两列，也就不满足了第三范式的设计：其他列之间不能有传递依赖关系。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">myorder</span> (
    order_id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    product_id <span class="pl-k">INT</span>,
    customer_id <span class="pl-k">INT</span>
);

<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">customer</span> (
    id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    phone <span class="pl-k">VARCHAR</span>(<span class="pl-c1">15</span>)
);</pre></div>
<p>修改后就不存在其他列之间的传递依赖关系，其他列都只依赖于主键列，满足了第三范式的设计！</p>
<h2><a id="user-content-查询练习" class="anchor" aria-hidden="true" href="#查询练习"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>查询练习</h2>
<h3><a id="user-content-准备数据" class="anchor" aria-hidden="true" href="#准备数据"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>准备数据</h3>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 创建数据库</span>
<span class="pl-k">CREATE</span> <span class="pl-k">DATABASE</span> <span class="pl-en">select_test</span>;
<span class="pl-c"><span class="pl-c">--</span> 切换数据库</span>
USE select_test;

<span class="pl-c"><span class="pl-c">--</span> 创建学生表</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">student</span> (
    no <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">NOT NULL</span>,
    sex <span class="pl-k">VARCHAR</span>(<span class="pl-c1">10</span>) <span class="pl-k">NOT NULL</span>,
    birthday <span class="pl-k">DATE</span>, <span class="pl-c"><span class="pl-c">--</span> 生日</span>
    class <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-c"><span class="pl-c">--</span> 所在班级</span>
);

<span class="pl-c"><span class="pl-c">--</span> 创建教师表</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">teacher</span> (
    no <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">NOT NULL</span>,
    sex <span class="pl-k">VARCHAR</span>(<span class="pl-c1">10</span>) <span class="pl-k">NOT NULL</span>,
    birthday <span class="pl-k">DATE</span>,
    profession <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">NOT NULL</span>, <span class="pl-c"><span class="pl-c">--</span> 职称</span>
    department <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">NOT NULL</span> <span class="pl-c"><span class="pl-c">--</span> 部门</span>
);

<span class="pl-c"><span class="pl-c">--</span> 创建课程表</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">course</span> (
    no <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">NOT NULL</span>,
    t_no <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">NOT NULL</span>, <span class="pl-c"><span class="pl-c">--</span> 教师编号</span>
    <span class="pl-c"><span class="pl-c">--</span> 表示该 tno 来自于 teacher 表中的 no 字段值</span>
    <span class="pl-k">FOREIGN KEY</span>(t_no) <span class="pl-k">REFERENCES</span> teacher(no) 
);

<span class="pl-c"><span class="pl-c">--</span> 成绩表</span>
<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">score</span> (
    s_no <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">NOT NULL</span>, <span class="pl-c"><span class="pl-c">--</span> 学生编号</span>
    c_no <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>) <span class="pl-k">NOT NULL</span>, <span class="pl-c"><span class="pl-c">--</span> 课程号</span>
    degree <span class="pl-k">DECIMAL</span>,	<span class="pl-c"><span class="pl-c">--</span> 成绩</span>
    <span class="pl-c"><span class="pl-c">--</span> 表示该 s_no, c_no 分别来自于 student, course 表中的 no 字段值</span>
    <span class="pl-k">FOREIGN KEY</span>(s_no) <span class="pl-k">REFERENCES</span> student(no),	
    <span class="pl-k">FOREIGN KEY</span>(c_no) <span class="pl-k">REFERENCES</span> course(no),
    <span class="pl-c"><span class="pl-c">--</span> 设置 s_no, c_no 为联合主键</span>
    <span class="pl-k">PRIMARY KEY</span>(s_no, c_no)
);

<span class="pl-c"><span class="pl-c">--</span> 查看所有表</span>
SHOW TABLES;

<span class="pl-c"><span class="pl-c">--</span> 添加学生表数据</span>
<span class="pl-k">INSERT INTO</span> student <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>101<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>曾华<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1977-09-01<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>95033<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> student <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>102<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>匡明<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1975-10-02<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>95031<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> student <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>103<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>王丽<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>女<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1976-01-23<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>95033<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> student <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>104<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>李军<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1976-02-20<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>95033<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> student <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>王芳<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>女<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1975-02-10<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>95031<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> student <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>106<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>陆军<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1974-06-03<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>95031<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> student <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>107<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>王尼玛<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1976-02-20<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>95033<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> student <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>108<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>张全蛋<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1975-02-10<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>95031<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> student <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>109<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>赵铁柱<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1974-06-03<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>95031<span class="pl-pds">'</span></span>);

<span class="pl-c"><span class="pl-c">--</span> 添加教师表数据</span>
<span class="pl-k">INSERT INTO</span> teacher <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>804<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>李诚<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1958-12-02<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>副教授<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>计算机系<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> teacher <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>856<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>张旭<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1969-03-12<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>讲师<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>电子工程系<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> teacher <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>825<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>王萍<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>女<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1972-05-05<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>助教<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>计算机系<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> teacher <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>831<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>刘冰<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>女<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>1977-08-14<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>助教<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>电子工程系<span class="pl-pds">'</span></span>);

<span class="pl-c"><span class="pl-c">--</span> 添加课程表数据</span>
<span class="pl-k">INSERT INTO</span> course <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>计算机导论<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>825<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> course <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>3-245<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>操作系统<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>804<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> course <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>6-166<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>数字电路<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>856<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> course <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>9-888<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>高等数学<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>831<span class="pl-pds">'</span></span>);

<span class="pl-c"><span class="pl-c">--</span> 添加添加成绩表数据</span>
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>103<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>92<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>103<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>3-245<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>86<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>103<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>6-166<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>85<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>88<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>3-245<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>75<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>6-166<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>79<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>109<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>76<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>109<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>3-245<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>68<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span>(<span class="pl-s"><span class="pl-pds">'</span>109<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>6-166<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>81<span class="pl-pds">'</span></span>);

<span class="pl-c"><span class="pl-c">--</span> 查看表结构</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> course;
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score;
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> student;
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> teacher;</pre></div>
<h3><a id="user-content-1-到-10" class="anchor" aria-hidden="true" href="#1-到-10"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>1 到 10</h3>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 查询 student 表的所有行</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> student;

<span class="pl-c"><span class="pl-c">--</span> 查询 student 表中的 name、sex 和 class 字段的所有行</span>
<span class="pl-k">SELECT</span> name, sex, class <span class="pl-k">FROM</span> student;

<span class="pl-c"><span class="pl-c">--</span> 查询 teacher 表中不重复的 department 列</span>
<span class="pl-c"><span class="pl-c">--</span> department: 去重查询</span>
<span class="pl-k">SELECT DISTINCT</span> department <span class="pl-k">FROM</span> teacher;

<span class="pl-c"><span class="pl-c">--</span> 查询 score 表中成绩在60-80之间的所有行（区间查询和运算符查询）</span>
<span class="pl-c"><span class="pl-c">--</span> BETWEEN xx AND xx: 查询区间, AND 表示 "并且"</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> degree BETWEEN <span class="pl-c1">60</span> <span class="pl-k">AND</span> <span class="pl-c1">80</span>;
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> degree <span class="pl-k">&gt;</span> <span class="pl-c1">60</span> <span class="pl-k">AND</span> degree <span class="pl-k">&lt;</span> <span class="pl-c1">80</span>;

<span class="pl-c"><span class="pl-c">--</span> 查询 score 表中成绩为 85, 86 或 88 的行</span>
<span class="pl-c"><span class="pl-c">--</span> IN: 查询规定中的多个值</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> degree <span class="pl-k">IN</span> (<span class="pl-c1">85</span>, <span class="pl-c1">86</span>, <span class="pl-c1">88</span>);

<span class="pl-c"><span class="pl-c">--</span> 查询 student 表中 '95031' 班或性别为 '女' 的所有行</span>
<span class="pl-c"><span class="pl-c">--</span> or: 表示或者关系</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> class <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>95031<span class="pl-pds">'</span></span> <span class="pl-k">or</span> sex <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>女<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> 以 class 降序的方式查询 student 表的所有行</span>
<span class="pl-c"><span class="pl-c">--</span> DESC: 降序，从高到低</span>
<span class="pl-c"><span class="pl-c">--</span> ASC（默认）: 升序，从低到高</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> student <span class="pl-k">ORDER BY</span> class <span class="pl-k">DESC</span>;
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> student <span class="pl-k">ORDER BY</span> class <span class="pl-k">ASC</span>;

<span class="pl-c"><span class="pl-c">--</span> 以 c_no 升序、degree 降序查询 score 表的所有行</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">ORDER BY</span> c_no <span class="pl-k">ASC</span>, degree <span class="pl-k">DESC</span>;

<span class="pl-c"><span class="pl-c">--</span> 查询 "95031" 班的学生人数</span>
<span class="pl-c"><span class="pl-c">--</span> COUNT: 统计</span>
<span class="pl-k">SELECT</span> <span class="pl-c1">COUNT</span>(<span class="pl-k">*</span>) <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> class <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>95031<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> 查询 score 表中的最高分的学生学号和课程编号（子查询或排序查询）。</span>
<span class="pl-c"><span class="pl-c">--</span> (SELECT MAX(degree) FROM score): 子查询，算出最高分</span>
<span class="pl-k">SELECT</span> s_no, c_no <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> degree <span class="pl-k">=</span> (<span class="pl-k">SELECT</span> <span class="pl-c1">MAX</span>(degree) <span class="pl-k">FROM</span> score);

<span class="pl-c"><span class="pl-c">--</span>  排序查询</span>
<span class="pl-c"><span class="pl-c">--</span> LIMIT r, n: 表示从第r行开始，查询n条数据</span>
<span class="pl-k">SELECT</span> s_no, c_no, degree <span class="pl-k">FROM</span> score <span class="pl-k">ORDER BY</span> degree <span class="pl-k">DESC</span> <span class="pl-k">LIMIT</span> <span class="pl-c1">0</span>, <span class="pl-c1">1</span>;</pre></div>
<h3><a id="user-content-分组计算平均成绩" class="anchor" aria-hidden="true" href="#分组计算平均成绩"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>分组计算平均成绩</h3>
<p><strong>查询每门课的平均成绩。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> AVG: 平均值</span>
<span class="pl-k">SELECT</span> <span class="pl-c1">AVG</span>(degree) <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>;
<span class="pl-k">SELECT</span> <span class="pl-c1">AVG</span>(degree) <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-245<span class="pl-pds">'</span></span>;
<span class="pl-k">SELECT</span> <span class="pl-c1">AVG</span>(degree) <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>6-166<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> GROUP BY: 分组查询</span>
<span class="pl-k">SELECT</span> c_no, <span class="pl-c1">AVG</span>(degree) <span class="pl-k">FROM</span> score <span class="pl-k">GROUP BY</span> c_no;</pre></div>
<h3><a id="user-content-分组条件与模糊查询" class="anchor" aria-hidden="true" href="#分组条件与模糊查询"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>分组条件与模糊查询</h3>
<p><strong>查询 <code>score</code> 表中至少有 2 名学生选修，并以 3 开头的课程的平均分数。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score;
<span class="pl-c"><span class="pl-c">--</span> c_no 课程编号</span>
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">86</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">85</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">79</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<p>分析表发现，至少有 2 名学生选修的课程是 <code>3-105</code> 、<code>3-245</code> 、<code>6-166</code> ，以 3 开头的课程是 <code>3-105</code> 、<code>3-245</code> 。也就是说，我们要查询所有 <code>3-105</code> 和 <code>3-245</code> 的 <code>degree</code> 平均分。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 首先把 c_no, AVG(degree) 通过分组查询出来</span>
<span class="pl-k">SELECT</span> c_no, <span class="pl-c1">AVG</span>(degree) <span class="pl-k">FROM</span> score <span class="pl-k">GROUP BY</span> c_no
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+</span>
| c_no  | <span class="pl-c1">AVG</span>(degree) |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">85</span>.<span class="pl-c1">3333</span> |
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">76</span>.<span class="pl-c1">3333</span> |
| <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span>.<span class="pl-c1">6667</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+</span>

<span class="pl-c"><span class="pl-c">--</span> 再查询出至少有 2 名学生选修的课程</span>
<span class="pl-c"><span class="pl-c">--</span> HAVING: 表示持有</span>
<span class="pl-k">HAVING</span> <span class="pl-c1">COUNT</span>(c_no) <span class="pl-k">&gt;=</span> <span class="pl-c1">2</span>

<span class="pl-c"><span class="pl-c">--</span> 并且是以 3 开头的课程</span>
<span class="pl-c"><span class="pl-c">--</span> LIKE 表示模糊查询，"%" 是一个通配符，匹配 "3" 后面的任意字符。</span>
<span class="pl-k">AND</span> c_no <span class="pl-k">LIKE</span> <span class="pl-s"><span class="pl-pds">'</span>3%<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> 把前面的SQL语句拼接起来，</span>
<span class="pl-c"><span class="pl-c">--</span> 后面加上一个 COUNT(*)，表示将每个分组的个数也查询出来。</span>
<span class="pl-k">SELECT</span> c_no, <span class="pl-c1">AVG</span>(degree), <span class="pl-c1">COUNT</span>(<span class="pl-k">*</span>) <span class="pl-k">FROM</span> score <span class="pl-k">GROUP BY</span> c_no
<span class="pl-k">HAVING</span> <span class="pl-c1">COUNT</span>(c_no) <span class="pl-k">&gt;=</span> <span class="pl-c1">2</span> <span class="pl-k">AND</span> c_no <span class="pl-k">LIKE</span> <span class="pl-s"><span class="pl-pds">'</span>3%<span class="pl-pds">'</span></span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+----------+</span>
| c_no  | <span class="pl-c1">AVG</span>(degree) | <span class="pl-c1">COUNT</span>(<span class="pl-k">*</span>) |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+----------+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">85</span>.<span class="pl-c1">3333</span> |        <span class="pl-c1">3</span> |
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">76</span>.<span class="pl-c1">3333</span> |        <span class="pl-c1">3</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+----------+</span></pre></div>
<h3><a id="user-content-多表查询---1" class="anchor" aria-hidden="true" href="#多表查询---1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>多表查询 - 1</h3>
<p><strong>查询所有学生的 <code>name</code>，以及该学生在 <code>score</code> 表中对应的 <code>c_no</code> 和 <code>degree</code> 。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> no, name <span class="pl-k">FROM</span> student;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+</span>
| no  | name      |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+</span>
| <span class="pl-c1">101</span> | 曾华      |
| <span class="pl-c1">102</span> | 匡明      |
| <span class="pl-c1">103</span> | 王丽      |
| <span class="pl-c1">104</span> | 李军      |
| <span class="pl-c1">105</span> | 王芳      |
| <span class="pl-c1">106</span> | 陆军      |
| <span class="pl-c1">107</span> | 王尼玛    |
| <span class="pl-c1">108</span> | 张全蛋    |
| <span class="pl-c1">109</span> | 赵铁柱    |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+</span>

<span class="pl-k">SELECT</span> s_no, c_no, degree <span class="pl-k">FROM</span> score;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">86</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">85</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">79</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<p>通过分析可以发现，只要把 <code>score</code> 表中的 <code>s_no</code> 字段值替换成 <code>student</code> 表中对应的 <code>name</code> 字段值就可以了，如何做呢？</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> FROM...: 表示从 student, score 表中查询</span>
<span class="pl-c"><span class="pl-c">--</span> WHERE 的条件表示为，只有在 student.no 和 score.s_no 相等时才显示出来。</span>
<span class="pl-k">SELECT</span> name, c_no, degree <span class="pl-k">FROM</span> student, score 
<span class="pl-k">WHERE</span> <span class="pl-c1">student</span>.<span class="pl-c1">no</span> <span class="pl-k">=</span> <span class="pl-c1">score</span>.<span class="pl-c1">s_no</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-------+--------+</span>
| name      | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-------+--------+</span>
| 王丽      | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| 王丽      | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">86</span> |
| 王丽      | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">85</span> |
| 王芳      | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| 王芳      | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| 王芳      | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">79</span> |
| 赵铁柱    | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
| 赵铁柱    | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| 赵铁柱    | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-------+--------+</span></pre></div>
<h3><a id="user-content-多表查询---2" class="anchor" aria-hidden="true" href="#多表查询---2"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>多表查询 - 2</h3>
<p><strong>查询所有学生的 <code>no</code> 、课程名称 ( <code>course</code> 表中的 <code>name</code> ) 和成绩 ( <code>score</code> 表中的 <code>degree</code> ) 列。</strong></p>
<p>只有 <code>score</code> 关联学生的 <code>no</code> ，因此只要查询 <code>score</code> 表，就能找出所有和学生相关的 <code>no</code> 和 <code>degree</code> ：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> s_no, c_no, degree <span class="pl-k">FROM</span> score;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">86</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">85</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">79</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<p>然后查询 <code>course</code> 表：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-----------------+</span>
| no    | name            |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-----------------+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> | 计算机导论      |
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> | 操作系统        |
| <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> | 数字电路        |
| <span class="pl-c1">9</span><span class="pl-k">-</span><span class="pl-c1">888</span> | 高等数学        |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-----------------+</span></pre></div>
<p>只要把 <code>score</code> 表中的 <code>c_no</code> 替换成 <code>course</code> 表中对应的 <code>name</code> 字段值就可以了。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 增加一个查询字段 name，分别从 score、course 这两个表中查询。</span>
<span class="pl-c"><span class="pl-c">--</span> as 表示取一个该字段的别名。</span>
<span class="pl-k">SELECT</span> s_no, name <span class="pl-k">as</span> c_name, degree <span class="pl-k">FROM</span> score, course
<span class="pl-k">WHERE</span> <span class="pl-c1">score</span>.<span class="pl-c1">c_no</span> <span class="pl-k">=</span> <span class="pl-c1">course</span>.<span class="pl-c1">no</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-----------------+--------+</span>
| s_no | c_name          | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-----------------+--------+</span>
| <span class="pl-c1">103</span>  | 计算机导论      |     <span class="pl-c1">92</span> |
| <span class="pl-c1">105</span>  | 计算机导论      |     <span class="pl-c1">88</span> |
| <span class="pl-c1">109</span>  | 计算机导论      |     <span class="pl-c1">76</span> |
| <span class="pl-c1">103</span>  | 操作系统        |     <span class="pl-c1">86</span> |
| <span class="pl-c1">105</span>  | 操作系统        |     <span class="pl-c1">75</span> |
| <span class="pl-c1">109</span>  | 操作系统        |     <span class="pl-c1">68</span> |
| <span class="pl-c1">103</span>  | 数字电路        |     <span class="pl-c1">85</span> |
| <span class="pl-c1">105</span>  | 数字电路        |     <span class="pl-c1">79</span> |
| <span class="pl-c1">109</span>  | 数字电路        |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-----------------+--------+</span></pre></div>
<h3><a id="user-content-三表关联查询" class="anchor" aria-hidden="true" href="#三表关联查询"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>三表关联查询</h3>
<p><strong>查询所有学生的 <code>name</code> 、课程名 ( <code>course</code> 表中的 <code>name</code> ) 和 <code>degree</code> 。</strong></p>
<p>只有 <code>score</code> 表中关联学生的学号和课堂号，我们只要围绕着 <code>score</code> 这张表查询就好了。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">86</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">85</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">79</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<p>只要把 <code>s_no</code> 和 <code>c_no</code> 替换成 <code>student</code> 和 <code>srouse</code> 表中对应的 <code>name</code> 字段值就好了。</p>
<p>首先把 <code>s_no</code> 替换成 <code>student</code> 表中的 <code>name</code> 字段：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> name, c_no, degree <span class="pl-k">FROM</span> student, score <span class="pl-k">WHERE</span> <span class="pl-c1">student</span>.<span class="pl-c1">no</span> <span class="pl-k">=</span> <span class="pl-c1">score</span>.<span class="pl-c1">s_no</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-------+--------+</span>
| name      | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-------+--------+</span>
| 王丽      | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| 王丽      | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">86</span> |
| 王丽      | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">85</span> |
| 王芳      | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| 王芳      | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| 王芳      | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">79</span> |
| 赵铁柱    | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
| 赵铁柱    | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| 赵铁柱    | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-------+--------+</span></pre></div>
<p>再把 <code>c_no</code> 替换成 <code>course</code> 表中的 <code>name</code> 字段：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 课程表</span>
<span class="pl-k">SELECT</span> no, name <span class="pl-k">FROM</span> course;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-----------------+</span>
| no    | name            |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-----------------+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> | 计算机导论      |
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> | 操作系统        |
| <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> | 数字电路        |
| <span class="pl-c1">9</span><span class="pl-k">-</span><span class="pl-c1">888</span> | 高等数学        |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-----------------+</span>

<span class="pl-c"><span class="pl-c">--</span> 由于字段名存在重复，使用 "表名.字段名 as 别名" 代替。</span>
<span class="pl-k">SELECT</span> <span class="pl-c1">student</span>.<span class="pl-c1">name</span> <span class="pl-k">as</span> s_name, <span class="pl-c1">course</span>.<span class="pl-c1">name</span> <span class="pl-k">as</span> c_name, degree 
<span class="pl-k">FROM</span> student, score, course
<span class="pl-k">WHERE</span> <span class="pl-c1">student</span>.<span class="pl-c1">NO</span> <span class="pl-k">=</span> <span class="pl-c1">score</span>.<span class="pl-c1">s_no</span>
<span class="pl-k">AND</span> <span class="pl-c1">score</span>.<span class="pl-c1">c_no</span> <span class="pl-k">=</span> <span class="pl-c1">course</span>.<span class="pl-c1">no</span>;</pre></div>
<h3><a id="user-content-子查询加分组求平均分" class="anchor" aria-hidden="true" href="#子查询加分组求平均分"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>子查询加分组求平均分</h3>
<p><strong>查询 <code>95031</code> 班学生每门课程的平均成绩。</strong></p>
<p>在 <code>score</code> 表中根据 <code>student</code>  表的学生编号筛选出学生的课堂号和成绩：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> IN (..): 将筛选出的学生号当做 s_no 的条件查询</span>
<span class="pl-k">SELECT</span> s_no, c_no, degree <span class="pl-k">FROM</span> score
<span class="pl-k">WHERE</span> s_no <span class="pl-k">IN</span> (<span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> class <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>95031<span class="pl-pds">'</span></span>);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">79</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<p>这时只要将 <code>c_no</code> 分组一下就能得出 <code>95031</code> 班学生每门课的平均成绩：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> c_no, <span class="pl-c1">AVG</span>(degree) <span class="pl-k">FROM</span> score
<span class="pl-k">WHERE</span> s_no <span class="pl-k">IN</span> (<span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> class <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>95031<span class="pl-pds">'</span></span>)
<span class="pl-k">GROUP BY</span> c_no;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+</span>
| c_no  | <span class="pl-c1">AVG</span>(degree) |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">82</span>.<span class="pl-c1">0000</span> |
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">71</span>.<span class="pl-c1">5000</span> |
| <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">80</span>.<span class="pl-c1">0000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+</span></pre></div>
<h3><a id="user-content-子查询---1" class="anchor" aria-hidden="true" href="#子查询---1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>子查询 - 1</h3>
<p><strong>查询在 <code>3-105</code> 课程中，所有成绩高于 <code>109</code> 号同学的记录。</strong></p>
<p>首先筛选出课堂号为 <code>3-105</code> ，在找出所有成绩高于 <code>109</code> 号同学的的行。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score 
<span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>
<span class="pl-k">AND</span> degree <span class="pl-k">&gt;</span> (<span class="pl-k">SELECT</span> degree <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> s_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>109<span class="pl-pds">'</span></span> <span class="pl-k">AND</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>);</pre></div>
<h3><a id="user-content-子查询---2" class="anchor" aria-hidden="true" href="#子查询---2"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>子查询 - 2</h3>
<p><strong>查询所有成绩高于 <code>109</code> 号同学的 <code>3-105</code> 课程成绩记录。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 不限制课程号，只要成绩大于109号同学的3-105课程成绩就可以。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score
<span class="pl-k">WHERE</span> degree <span class="pl-k">&gt;</span> (<span class="pl-k">SELECT</span> degree <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> s_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>109<span class="pl-pds">'</span></span> <span class="pl-k">AND</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>);</pre></div>
<h3><a id="user-content-year-函数与带-in-关键字查询" class="anchor" aria-hidden="true" href="#year-函数与带-in-关键字查询"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>YEAR 函数与带 IN 关键字查询</h3>
<p><strong>查询所有和 <code>101</code> 、<code>108</code> 号学生同年出生的 <code>no</code> 、<code>name</code> 、<code>birthday</code> 列。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> YEAR(..): 取出日期中的年份</span>
<span class="pl-k">SELECT</span> no, name, birthday <span class="pl-k">FROM</span> student
<span class="pl-k">WHERE</span> YEAR(birthday) <span class="pl-k">IN</span> (<span class="pl-k">SELECT</span> YEAR(birthday) <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> no <span class="pl-k">IN</span> (<span class="pl-c1">101</span>, <span class="pl-c1">108</span>));</pre></div>
<h3><a id="user-content-多层嵌套子查询" class="anchor" aria-hidden="true" href="#多层嵌套子查询"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>多层嵌套子查询</h3>
<p><strong>查询 <code>'张旭'</code> 教师任课的学生成绩表。</strong></p>
<p>首先找到教师编号：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> NO <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> NAME <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>张旭<span class="pl-pds">'</span></span></pre></div>
<p>通过 <code>sourse</code> 表找到该教师课程号：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> NO <span class="pl-k">FROM</span> course <span class="pl-k">WHERE</span> t_no <span class="pl-k">=</span> ( <span class="pl-k">SELECT</span> NO <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> NAME <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>张旭<span class="pl-pds">'</span></span> );</pre></div>
<p>通过筛选出的课程号查询成绩表：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> (
    <span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> course <span class="pl-k">WHERE</span> t_no <span class="pl-k">=</span> ( 
        <span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> NAME <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>张旭<span class="pl-pds">'</span></span> 
    )
);</pre></div>
<h3><a id="user-content-多表查询" class="anchor" aria-hidden="true" href="#多表查询"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>多表查询</h3>
<p><strong>查询某选修课程多于5个同学的教师姓名。</strong></p>
<p>首先在 <code>teacher</code> 表中，根据 <code>no</code> 字段来判断该教师的同一门课程是否有至少5名学员选修：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 查询 teacher 表</span>
<span class="pl-k">SELECT</span> no, name <span class="pl-k">FROM</span> teacher;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+--------+</span>
| no  | name   |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+--------+</span>
| <span class="pl-c1">804</span> | 李诚   |
| <span class="pl-c1">825</span> | 王萍   |
| <span class="pl-c1">831</span> | 刘冰   |
| <span class="pl-c1">856</span> | 张旭   |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+--------+</span>

<span class="pl-k">SELECT</span> name <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> no <span class="pl-k">IN</span> (
    <span class="pl-c"><span class="pl-c">--</span> 在这里找到对应的条件</span>
);</pre></div>
<p>查看和教师编号有有关的表的信息：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> course;
<span class="pl-c"><span class="pl-c">--</span> t_no: 教师编号</span>
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-----------------+------+</span>
| no    | name            | t_no |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-----------------+------+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> | 计算机导论      | <span class="pl-c1">825</span>  |
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> | 操作系统        | <span class="pl-c1">804</span>  |
| <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> | 数字电路        | <span class="pl-c1">856</span>  |
| <span class="pl-c1">9</span><span class="pl-k">-</span><span class="pl-c1">888</span> | 高等数学        | <span class="pl-c1">831</span>  |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-----------------+------+</span></pre></div>
<p>我们已经找到和教师编号有关的字段就在 <code>course</code> 表中，但是还无法知道哪门课程至少有5名学生选修，所以还需要根据 <code>score</code> 表来查询：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 在此之前向 score 插入一些数据，以便丰富查询条件。</span>
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>101<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>90<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>102<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>91<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> score <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>104<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>89<span class="pl-pds">'</span></span>);

<span class="pl-c"><span class="pl-c">--</span> 查询 score 表</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">101</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">90</span> |
| <span class="pl-c1">102</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">91</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">86</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">85</span> |
| <span class="pl-c1">104</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">89</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">79</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>

<span class="pl-c"><span class="pl-c">--</span> 在 score 表中将 c_no 作为分组，并且限制 c_no 持有至少 5 条数据。</span>
<span class="pl-k">SELECT</span> c_no <span class="pl-k">FROM</span> score <span class="pl-k">GROUP BY</span> c_no <span class="pl-k">HAVING</span> <span class="pl-c1">COUNT</span>(<span class="pl-k">*</span>) <span class="pl-k">&gt;</span> <span class="pl-c1">5</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+</span>
| c_no  |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+</span></pre></div>
<p>根据筛选出来的课程号，找出在某课程中，拥有至少5名学员的教师编号：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> t_no <span class="pl-k">FROM</span> course <span class="pl-k">WHERE</span> no <span class="pl-k">IN</span> (
    <span class="pl-k">SELECT</span> c_no <span class="pl-k">FROM</span> score <span class="pl-k">GROUP BY</span> c_no <span class="pl-k">HAVING</span> <span class="pl-c1">COUNT</span>(<span class="pl-k">*</span>) <span class="pl-k">&gt;</span> <span class="pl-c1">5</span>
);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+</span>
| t_no |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+</span>
| <span class="pl-c1">825</span>  |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+</span></pre></div>
<p>在 <code>teacher</code> 表中，根据筛选出来的教师编号找到教师姓名：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> name <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> no <span class="pl-k">IN</span> (
    <span class="pl-c"><span class="pl-c">--</span> 最终条件</span>
    <span class="pl-k">SELECT</span> t_no <span class="pl-k">FROM</span> course <span class="pl-k">WHERE</span> no <span class="pl-k">IN</span> (
        <span class="pl-k">SELECT</span> c_no <span class="pl-k">FROM</span> score <span class="pl-k">GROUP BY</span> c_no <span class="pl-k">HAVING</span> <span class="pl-c1">COUNT</span>(<span class="pl-k">*</span>) <span class="pl-k">&gt;</span> <span class="pl-c1">5</span>
    )
);</pre></div>
<h3><a id="user-content-子查询---3" class="anchor" aria-hidden="true" href="#子查询---3"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>子查询 - 3</h3>
<p><strong>查询 “计算机系” 课程的成绩表。</strong></p>
<p>思路是，先找出 <code>course</code> 表中所有 <code>计算机系</code> 课程的编号，然后根据这个编号查询 <code>score</code> 表。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 通过 teacher 表查询所有 `计算机系` 的教师编号</span>
<span class="pl-k">SELECT</span> no, name, department <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> department <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>计算机系<span class="pl-pds">'</span></span>
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+--------+--------------+</span>
| no  | name   | department   |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+--------+--------------+</span>
| <span class="pl-c1">804</span> | 李诚   | 计算机系     |
| <span class="pl-c1">825</span> | 王萍   | 计算机系     |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+--------+--------------+</span>

<span class="pl-c"><span class="pl-c">--</span> 通过 course 表查询该教师的课程编号</span>
<span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> course <span class="pl-k">WHERE</span> t_no <span class="pl-k">IN</span> (
    <span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> department <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>计算机系<span class="pl-pds">'</span></span>
);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+</span>
| no    |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+</span>

<span class="pl-c"><span class="pl-c">--</span> 根据筛选出来的课程号查询成绩表</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">IN</span> (
    <span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> course <span class="pl-k">WHERE</span> t_no <span class="pl-k">IN</span> (
        <span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> department <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>计算机系<span class="pl-pds">'</span></span>
    )
);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">86</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| <span class="pl-c1">101</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">90</span> |
| <span class="pl-c1">102</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">91</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| <span class="pl-c1">104</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">89</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<h3><a id="user-content-union-和-notin-的使用" class="anchor" aria-hidden="true" href="#union-和-notin-的使用"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>UNION 和 NOTIN 的使用</h3>
<p><strong>查询 <code>计算机系</code> 与 <code>电子工程系</code> 中的不同职称的教师。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> NOT: 代表逻辑非</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> department <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>计算机系<span class="pl-pds">'</span></span> <span class="pl-k">AND</span> profession NOT <span class="pl-k">IN</span> (
    <span class="pl-k">SELECT</span> profession <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> department <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>电子工程系<span class="pl-pds">'</span></span>
)
<span class="pl-c"><span class="pl-c">--</span> 合并两个集</span>
<span class="pl-k">UNION</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> department <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>电子工程系<span class="pl-pds">'</span></span> <span class="pl-k">AND</span> profession NOT <span class="pl-k">IN</span> (
    <span class="pl-k">SELECT</span> profession <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> department <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>计算机系<span class="pl-pds">'</span></span>
);</pre></div>
<h3><a id="user-content-any-表示至少一个---desc--降序-" class="anchor" aria-hidden="true" href="#any-表示至少一个---desc--降序-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>ANY 表示至少一个 - DESC ( 降序 )</h3>
<p><strong>查询课程 <code>3-105</code> 且成绩 至少 高于 <code>3-245</code> 的 <code>score</code> 表。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">101</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">90</span> |
| <span class="pl-c1">102</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">91</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| <span class="pl-c1">104</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">89</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>

<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-245<span class="pl-pds">'</span></span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">86</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>

<span class="pl-c"><span class="pl-c">--</span> ANY: 符合SQL语句中的任意条件。</span>
<span class="pl-c"><span class="pl-c">--</span> 也就是说，在 3-105 成绩中，只要有一个大于从 3-245 筛选出来的任意行就符合条件，</span>
<span class="pl-c"><span class="pl-c">--</span> 最后根据降序查询结果。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span> <span class="pl-k">AND</span> degree <span class="pl-k">&gt;</span> ANY(
    <span class="pl-k">SELECT</span> degree <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-245<span class="pl-pds">'</span></span>
) <span class="pl-k">ORDER BY</span> degree <span class="pl-k">DESC</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| <span class="pl-c1">102</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">91</span> |
| <span class="pl-c1">101</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">90</span> |
| <span class="pl-c1">104</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">89</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<h3><a id="user-content-表示所有的-all" class="anchor" aria-hidden="true" href="#表示所有的-all"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>表示所有的 ALL</h3>
<p><strong>查询课程 <code>3-105</code> 且成绩高于 <code>3-245</code> 的 <code>score</code> 表。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 只需对上一道题稍作修改。</span>
<span class="pl-c"><span class="pl-c">--</span> ALL: 符合SQL语句中的所有条件。</span>
<span class="pl-c"><span class="pl-c">--</span> 也就是说，在 3-105 每一行成绩中，都要大于从 3-245 筛选出来全部行才算符合条件。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-105<span class="pl-pds">'</span></span> <span class="pl-k">AND</span> degree <span class="pl-k">&gt;</span> ALL(
    <span class="pl-k">SELECT</span> degree <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>3-245<span class="pl-pds">'</span></span>
);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">101</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">90</span> |
| <span class="pl-c1">102</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">91</span> |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
| <span class="pl-c1">104</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">89</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">88</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<h3><a id="user-content-复制表的数据作为条件查询" class="anchor" aria-hidden="true" href="#复制表的数据作为条件查询"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>复制表的数据作为条件查询</h3>
<p><strong>查询某课程成绩比该课程平均成绩低的 <code>score</code> 表。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 查询平均分</span>
<span class="pl-k">SELECT</span> c_no, <span class="pl-c1">AVG</span>(degree) <span class="pl-k">FROM</span> score <span class="pl-k">GROUP BY</span> c_no;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+</span>
| c_no  | <span class="pl-c1">AVG</span>(degree) |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">87</span>.<span class="pl-c1">6667</span> |
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">76</span>.<span class="pl-c1">3333</span> |
| <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span>.<span class="pl-c1">6667</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+-------------+</span>

<span class="pl-c"><span class="pl-c">--</span> 查询 score 表</span>
<span class="pl-k">SELECT</span> degree <span class="pl-k">FROM</span> score;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------+</span>
| degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------+</span>
|     <span class="pl-c1">90</span> |
|     <span class="pl-c1">91</span> |
|     <span class="pl-c1">92</span> |
|     <span class="pl-c1">86</span> |
|     <span class="pl-c1">85</span> |
|     <span class="pl-c1">89</span> |
|     <span class="pl-c1">88</span> |
|     <span class="pl-c1">75</span> |
|     <span class="pl-c1">79</span> |
|     <span class="pl-c1">76</span> |
|     <span class="pl-c1">68</span> |
|     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------+</span>

<span class="pl-c"><span class="pl-c">--</span> 将表 b 作用于表 a 中查询数据</span>
<span class="pl-c"><span class="pl-c">--</span> score a (b): 将表声明为 a (b)，</span>
<span class="pl-c"><span class="pl-c">--</span> 如此就能用 a.c_no = b.c_no 作为条件执行查询了。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score a <span class="pl-k">WHERE</span> degree <span class="pl-k">&lt;</span> (
    (<span class="pl-k">SELECT</span> <span class="pl-c1">AVG</span>(degree) <span class="pl-k">FROM</span> score b <span class="pl-k">WHERE</span> <span class="pl-c1">a</span>.<span class="pl-c1">c_no</span> <span class="pl-k">=</span> <span class="pl-c1">b</span>.<span class="pl-c1">c_no</span>)
);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">75</span> |
| <span class="pl-c1">105</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">79</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> |     <span class="pl-c1">68</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> |     <span class="pl-c1">81</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<h3><a id="user-content-子查询---4" class="anchor" aria-hidden="true" href="#子查询---4"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>子查询 - 4</h3>
<p><strong>查询所有任课 ( 在 <code>course</code> 表里有课程 ) 教师的 <code>name</code> 和 <code>department</code></strong> 。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> name, department <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> no <span class="pl-k">IN</span> (<span class="pl-k">SELECT</span> t_no <span class="pl-k">FROM</span> course);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------+-----------------+</span>
| name   | department      |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------+-----------------+</span>
| 李诚   | 计算机系        |
| 王萍   | 计算机系        |
| 刘冰   | 电子工程系      |
| 张旭   | 电子工程系      |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------+-----------------+</span></pre></div>
<h3><a id="user-content-条件加组筛选" class="anchor" aria-hidden="true" href="#条件加组筛选"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>条件加组筛选</h3>
<p><strong>查询 <code>student</code> 表中至少有 2 名男生的 <code>class</code> 。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 查看学生表信息</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> student;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+-----+------------+-------+</span>
| no  | name      | sex | birthday   | class |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+-----+------------+-------+</span>
| <span class="pl-c1">101</span> | 曾华      | 男  | <span class="pl-c1">1977</span><span class="pl-k">-</span><span class="pl-c1">09</span><span class="pl-k">-</span><span class="pl-c1">01</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">102</span> | 匡明      | 男  | <span class="pl-c1">1975</span><span class="pl-k">-</span><span class="pl-c1">10</span><span class="pl-k">-</span><span class="pl-c1">02</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">103</span> | 王丽      | 女  | <span class="pl-c1">1976</span><span class="pl-k">-</span><span class="pl-c1">01</span><span class="pl-k">-</span><span class="pl-c1">23</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">104</span> | 李军      | 男  | <span class="pl-c1">1976</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">20</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">105</span> | 王芳      | 女  | <span class="pl-c1">1975</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">10</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">106</span> | 陆军      | 男  | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">107</span> | 王尼玛    | 男  | <span class="pl-c1">1976</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">20</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">108</span> | 张全蛋    | 男  | <span class="pl-c1">1975</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">10</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">109</span> | 赵铁柱    | 男  | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">110</span> | 张飞      | 男  | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span> | <span class="pl-c1">95038</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+-----+------------+-------+</span>

<span class="pl-c"><span class="pl-c">--</span> 只查询性别为男，然后按 class 分组，并限制 class 行大于 1。</span>
<span class="pl-k">SELECT</span> class <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> sex <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span> <span class="pl-k">GROUP BY</span> class <span class="pl-k">HAVING</span> <span class="pl-c1">COUNT</span>(<span class="pl-k">*</span>) <span class="pl-k">&gt;</span> <span class="pl-c1">1</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+</span>
| class |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+</span>
| <span class="pl-c1">95033</span> |
| <span class="pl-c1">95031</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+</span></pre></div>
<h3><a id="user-content-notlike-模糊查询取反" class="anchor" aria-hidden="true" href="#notlike-模糊查询取反"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>NOTLIKE 模糊查询取反</h3>
<p><strong>查询 <code>student</code> 表中不姓 "王" 的同学记录。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> NOT: 取反</span>
<span class="pl-c"><span class="pl-c">--</span> LIKE: 模糊查询</span>
mysql<span class="pl-k">&gt;</span> <span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> name NOT <span class="pl-k">LIKE</span> <span class="pl-s"><span class="pl-pds">'</span>王%<span class="pl-pds">'</span></span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+-----+------------+-------+</span>
| no  | name      | sex | birthday   | class |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+-----+------------+-------+</span>
| <span class="pl-c1">101</span> | 曾华      | 男  | <span class="pl-c1">1977</span><span class="pl-k">-</span><span class="pl-c1">09</span><span class="pl-k">-</span><span class="pl-c1">01</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">102</span> | 匡明      | 男  | <span class="pl-c1">1975</span><span class="pl-k">-</span><span class="pl-c1">10</span><span class="pl-k">-</span><span class="pl-c1">02</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">104</span> | 李军      | 男  | <span class="pl-c1">1976</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">20</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">106</span> | 陆军      | 男  | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">108</span> | 张全蛋    | 男  | <span class="pl-c1">1975</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">10</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">109</span> | 赵铁柱    | 男  | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">110</span> | 张飞      | 男  | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span> | <span class="pl-c1">95038</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+-----+------------+-------+</span></pre></div>
<h3><a id="user-content-year-与-now-函数" class="anchor" aria-hidden="true" href="#year-与-now-函数"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>YEAR 与 NOW 函数</h3>
<p><strong>查询 <code>student</code> 表中每个学生的姓名和年龄。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 使用函数 YEAR(NOW()) 计算出当前年份，减去出生年份后得出年龄。</span>
<span class="pl-k">SELECT</span> name, YEAR(NOW()) <span class="pl-k">-</span> YEAR(birthday) <span class="pl-k">as</span> age <span class="pl-k">FROM</span> student;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+------+</span>
| name      | age  |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+------+</span>
| 曾华      |   <span class="pl-c1">42</span> |
| 匡明      |   <span class="pl-c1">44</span> |
| 王丽      |   <span class="pl-c1">43</span> |
| 李军      |   <span class="pl-c1">43</span> |
| 王芳      |   <span class="pl-c1">44</span> |
| 陆军      |   <span class="pl-c1">45</span> |
| 王尼玛    |   <span class="pl-c1">43</span> |
| 张全蛋    |   <span class="pl-c1">44</span> |
| 赵铁柱    |   <span class="pl-c1">45</span> |
| 张飞      |   <span class="pl-c1">45</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+------+</span></pre></div>
<h3><a id="user-content-max-与-min-函数" class="anchor" aria-hidden="true" href="#max-与-min-函数"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>MAX 与 MIN 函数</h3>
<p><strong>查询 <code>student</code> 表中最大和最小的 <code>birthday</code> 值。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-c1">MAX</span>(birthday), <span class="pl-c1">MIN</span>(birthday) <span class="pl-k">FROM</span> student;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-------------+---------------+</span>
| <span class="pl-c1">MAX</span>(birthday) | <span class="pl-c1">MIN</span>(birthday) |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-------------+---------------+</span>
| <span class="pl-c1">1977</span><span class="pl-k">-</span><span class="pl-c1">09</span><span class="pl-k">-</span><span class="pl-c1">01</span>    | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span>    |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-------------+---------------+</span></pre></div>
<h3><a id="user-content-多段排序" class="anchor" aria-hidden="true" href="#多段排序"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>多段排序</h3>
<p><strong>以 <code>class</code> 和 <code>birthday</code> 从大到小的顺序查询 <code>student</code> 表。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> student <span class="pl-k">ORDER BY</span> class <span class="pl-k">DESC</span>, birthday;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+-----+------------+-------+</span>
| no  | name      | sex | birthday   | class |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+-----+------------+-------+</span>
| <span class="pl-c1">110</span> | 张飞      | 男  | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span> | <span class="pl-c1">95038</span> |
| <span class="pl-c1">103</span> | 王丽      | 女  | <span class="pl-c1">1976</span><span class="pl-k">-</span><span class="pl-c1">01</span><span class="pl-k">-</span><span class="pl-c1">23</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">104</span> | 李军      | 男  | <span class="pl-c1">1976</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">20</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">107</span> | 王尼玛    | 男  | <span class="pl-c1">1976</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">20</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">101</span> | 曾华      | 男  | <span class="pl-c1">1977</span><span class="pl-k">-</span><span class="pl-c1">09</span><span class="pl-k">-</span><span class="pl-c1">01</span> | <span class="pl-c1">95033</span> |
| <span class="pl-c1">106</span> | 陆军      | 男  | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">109</span> | 赵铁柱    | 男  | <span class="pl-c1">1974</span><span class="pl-k">-</span><span class="pl-c1">06</span><span class="pl-k">-</span><span class="pl-c1">03</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">105</span> | 王芳      | 女  | <span class="pl-c1">1975</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">10</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">108</span> | 张全蛋    | 男  | <span class="pl-c1">1975</span><span class="pl-k">-</span><span class="pl-c1">02</span><span class="pl-k">-</span><span class="pl-c1">10</span> | <span class="pl-c1">95031</span> |
| <span class="pl-c1">102</span> | 匡明      | 男  | <span class="pl-c1">1975</span><span class="pl-k">-</span><span class="pl-c1">10</span><span class="pl-k">-</span><span class="pl-c1">02</span> | <span class="pl-c1">95031</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+-----------+-----+------------+-------+</span></pre></div>
<h3><a id="user-content-子查询---5" class="anchor" aria-hidden="true" href="#子查询---5"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>子查询 - 5</h3>
<p><strong>查询 "男" 教师及其所上的课程。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> course <span class="pl-k">WHERE</span> t_no <span class="pl-k">in</span> (<span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> teacher <span class="pl-k">WHERE</span> sex <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+--------------+------+</span>
| no    | name         | t_no |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+--------------+------+</span>
| <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> | 操作系统     | <span class="pl-c1">804</span>  |
| <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> | 数字电路     | <span class="pl-c1">856</span>  |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>-----+--------------+------+</span></pre></div>
<h3><a id="user-content-max-函数与子查询" class="anchor" aria-hidden="true" href="#max-函数与子查询"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>MAX 函数与子查询</h3>
<p><strong>查询最高分同学的 <code>score</code> 表。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 找出最高成绩（该查询只能有一个结果）</span>
<span class="pl-k">SELECT</span> <span class="pl-c1">MAX</span>(degree) <span class="pl-k">FROM</span> score;

<span class="pl-c"><span class="pl-c">--</span> 根据上面的条件筛选出所有最高成绩表，</span>
<span class="pl-c"><span class="pl-c">--</span> 该查询可能有多个结果，假设 degree 值多次符合条件。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> degree <span class="pl-k">=</span> (<span class="pl-k">SELECT</span> <span class="pl-c1">MAX</span>(degree) <span class="pl-k">FROM</span> score);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">92</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<h3><a id="user-content-子查询---6" class="anchor" aria-hidden="true" href="#子查询---6"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>子查询 - 6</h3>
<p><strong>查询和 "李军" 同性别的所有同学 <code>name</code> 。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 首先将李军的性别作为条件取出来</span>
<span class="pl-k">SELECT</span> sex <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>李军<span class="pl-pds">'</span></span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+</span>
| sex |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+</span>
| 男  |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---+</span>

<span class="pl-c"><span class="pl-c">--</span> 根据性别查询 name 和 sex</span>
<span class="pl-k">SELECT</span> name, sex <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> sex <span class="pl-k">=</span> (
    <span class="pl-k">SELECT</span> sex <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>李军<span class="pl-pds">'</span></span>
);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-----+</span>
| name      | sex |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-----+</span>
| 曾华      | 男  |
| 匡明      | 男  |
| 李军      | 男  |
| 陆军      | 男  |
| 王尼玛    | 男  |
| 张全蛋    | 男  |
| 赵铁柱    | 男  |
| 张飞      | 男  |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-----+</span></pre></div>
<h3><a id="user-content-子查询---7" class="anchor" aria-hidden="true" href="#子查询---7"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>子查询 - 7</h3>
<p><strong>查询和 "李军" 同性别且同班的同学 <code>name</code> 。</strong></p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> name, sex, class <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> sex <span class="pl-k">=</span> (
    <span class="pl-k">SELECT</span> sex <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>李军<span class="pl-pds">'</span></span>
) <span class="pl-k">AND</span> class <span class="pl-k">=</span> (
    <span class="pl-k">SELECT</span> class <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>李军<span class="pl-pds">'</span></span>
);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-----+-------+</span>
| name      | sex | class |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-----+-------+</span>
| 曾华      | 男  | <span class="pl-c1">95033</span> |
| 李军      | 男  | <span class="pl-c1">95033</span> |
| 王尼玛    | 男  | <span class="pl-c1">95033</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>---------+-----+-------+</span></pre></div>
<h3><a id="user-content-子查询---8" class="anchor" aria-hidden="true" href="#子查询---8"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>子查询 - 8</h3>
<p><strong>查询所有选修 "计算机导论" 课程的 "男" 同学成绩表。</strong></p>
<p>需要的 "计算机导论" 和性别为 "男" 的编号可以在 <code>course</code> 和 <code>student</code> 表中找到。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> score <span class="pl-k">WHERE</span> c_no <span class="pl-k">=</span> (
    <span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> course <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>计算机导论<span class="pl-pds">'</span></span>
) <span class="pl-k">AND</span> s_no <span class="pl-k">IN</span> (
    <span class="pl-k">SELECT</span> no <span class="pl-k">FROM</span> student <span class="pl-k">WHERE</span> sex <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>男<span class="pl-pds">'</span></span>
);
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| s_no | c_no  | degree |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span>
| <span class="pl-c1">101</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">90</span> |
| <span class="pl-c1">102</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">91</span> |
| <span class="pl-c1">104</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">89</span> |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> |     <span class="pl-c1">76</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+--------+</span></pre></div>
<h3><a id="user-content-按等级查询" class="anchor" aria-hidden="true" href="#按等级查询"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>按等级查询</h3>
<p>建立一个 <code>grade</code> 表代表学生的成绩等级，并插入数据：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">grade</span> (
    low <span class="pl-k">INT</span>(<span class="pl-c1">3</span>),
    upp <span class="pl-k">INT</span>(<span class="pl-c1">3</span>),
    grade <span class="pl-k">char</span>(<span class="pl-c1">1</span>)
);

<span class="pl-k">INSERT INTO</span> grade <span class="pl-k">VALUES</span> (<span class="pl-c1">90</span>, <span class="pl-c1">100</span>, <span class="pl-s"><span class="pl-pds">'</span>A<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> grade <span class="pl-k">VALUES</span> (<span class="pl-c1">80</span>, <span class="pl-c1">89</span>, <span class="pl-s"><span class="pl-pds">'</span>B<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> grade <span class="pl-k">VALUES</span> (<span class="pl-c1">70</span>, <span class="pl-c1">79</span>, <span class="pl-s"><span class="pl-pds">'</span>C<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> grade <span class="pl-k">VALUES</span> (<span class="pl-c1">60</span>, <span class="pl-c1">69</span>, <span class="pl-s"><span class="pl-pds">'</span>D<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> grade <span class="pl-k">VALUES</span> (<span class="pl-c1">0</span>, <span class="pl-c1">59</span>, <span class="pl-s"><span class="pl-pds">'</span>E<span class="pl-pds">'</span></span>);

<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> grade;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+------+-------+</span>
| low  | upp  | grade |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+------+-------+</span>
|   <span class="pl-c1">90</span> |  <span class="pl-c1">100</span> | A     |
|   <span class="pl-c1">80</span> |   <span class="pl-c1">89</span> | B     |
|   <span class="pl-c1">70</span> |   <span class="pl-c1">79</span> | C     |
|   <span class="pl-c1">60</span> |   <span class="pl-c1">69</span> | D     |
|    <span class="pl-c1">0</span> |   <span class="pl-c1">59</span> | E     |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+------+-------+</span></pre></div>
<p><strong>查询所有学生的 <code>s_no</code> 、<code>c_no</code> 和 <code>grade</code> 列。</strong></p>
<p>思路是，使用区间 ( <code>BETWEEN</code> ) 查询，判断学生的成绩 ( <code>degree</code> )  在 <code>grade</code> 表的 <code>low</code> 和 <code>upp</code> 之间。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> s_no, c_no, grade <span class="pl-k">FROM</span> score, grade 
<span class="pl-k">WHERE</span> degree BETWEEN low <span class="pl-k">AND</span> upp;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+-------+</span>
| s_no | c_no  | grade |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+-------+</span>
| <span class="pl-c1">101</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> | A     |
| <span class="pl-c1">102</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> | A     |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> | A     |
| <span class="pl-c1">103</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> | B     |
| <span class="pl-c1">103</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> | B     |
| <span class="pl-c1">104</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> | B     |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> | B     |
| <span class="pl-c1">105</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> | C     |
| <span class="pl-c1">105</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> | C     |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">105</span> | C     |
| <span class="pl-c1">109</span>  | <span class="pl-c1">3</span><span class="pl-k">-</span><span class="pl-c1">245</span> | D     |
| <span class="pl-c1">109</span>  | <span class="pl-c1">6</span><span class="pl-k">-</span><span class="pl-c1">166</span> | B     |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-------+-------+</span></pre></div>
<h3><a id="user-content-连接查询" class="anchor" aria-hidden="true" href="#连接查询"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>连接查询</h3>
<p>准备用于测试连接查询的数据：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">CREATE</span> <span class="pl-k">DATABASE</span> <span class="pl-en">testJoin</span>;

<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">person</span> (
    id <span class="pl-k">INT</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    cardId <span class="pl-k">INT</span>
);

<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">card</span> (
    id <span class="pl-k">INT</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>)
);

<span class="pl-k">INSERT INTO</span> card <span class="pl-k">VALUES</span> (<span class="pl-c1">1</span>, <span class="pl-s"><span class="pl-pds">'</span>饭卡<span class="pl-pds">'</span></span>), (<span class="pl-c1">2</span>, <span class="pl-s"><span class="pl-pds">'</span>建行卡<span class="pl-pds">'</span></span>), (<span class="pl-c1">3</span>, <span class="pl-s"><span class="pl-pds">'</span>农行卡<span class="pl-pds">'</span></span>), (<span class="pl-c1">4</span>, <span class="pl-s"><span class="pl-pds">'</span>工商卡<span class="pl-pds">'</span></span>), (<span class="pl-c1">5</span>, <span class="pl-s"><span class="pl-pds">'</span>邮政卡<span class="pl-pds">'</span></span>);
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> card;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-----------+</span>
| id   | name      |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-----------+</span>
|    <span class="pl-c1">1</span> | 饭卡      |
|    <span class="pl-c1">2</span> | 建行卡    |
|    <span class="pl-c1">3</span> | 农行卡    |
|    <span class="pl-c1">4</span> | 工商卡    |
|    <span class="pl-c1">5</span> | 邮政卡    |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+-----------+</span>

<span class="pl-k">INSERT INTO</span> person <span class="pl-k">VALUES</span> (<span class="pl-c1">1</span>, <span class="pl-s"><span class="pl-pds">'</span>张三<span class="pl-pds">'</span></span>, <span class="pl-c1">1</span>), (<span class="pl-c1">2</span>, <span class="pl-s"><span class="pl-pds">'</span>李四<span class="pl-pds">'</span></span>, <span class="pl-c1">3</span>), (<span class="pl-c1">3</span>, <span class="pl-s"><span class="pl-pds">'</span>王五<span class="pl-pds">'</span></span>, <span class="pl-c1">6</span>);
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> person;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+</span>
| id   | name   | cardId |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+</span>
|    <span class="pl-c1">1</span> | 张三   |      <span class="pl-c1">1</span> |
|    <span class="pl-c1">2</span> | 李四   |      <span class="pl-c1">3</span> |
|    <span class="pl-c1">3</span> | 王五   |      <span class="pl-c1">6</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+</span></pre></div>
<p>分析两张表发现，<code>person</code> 表并没有为 <code>cardId</code> 字段设置一个在 <code>card</code> 表中对应的 <code>id</code> 外键。如果设置了的话，<code>person</code> 中 <code>cardId</code> 字段值为 <code>6</code> 的行就插不进去，因为该 <code>cardId</code> 值在 <code>card</code> 表中并没有。</p>
<h4><a id="user-content-内连接" class="anchor" aria-hidden="true" href="#内连接"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>内连接</h4>
<p>要查询这两张表中有关系的数据，可以使用 <code>INNER JOIN</code> ( 内连接 ) 将它们连接在一起。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> INNER JOIN: 表示为内连接，将两张表拼接在一起。</span>
<span class="pl-c"><span class="pl-c">--</span> on: 表示要执行某个条件。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> person <span class="pl-k">INNER JOIN</span> card <span class="pl-k">on</span> <span class="pl-c1">person</span>.<span class="pl-c1">cardId</span> <span class="pl-k">=</span> <span class="pl-c1">card</span>.<span class="pl-c1">id</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span>
| id   | name   | cardId | id   | name      |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span>
|    <span class="pl-c1">1</span> | 张三   |      <span class="pl-c1">1</span> |    <span class="pl-c1">1</span> | 饭卡      |
|    <span class="pl-c1">2</span> | 李四   |      <span class="pl-c1">3</span> |    <span class="pl-c1">3</span> | 农行卡    |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span>

<span class="pl-c"><span class="pl-c">--</span> 将 INNER 关键字省略掉，结果也是一样的。</span>
<span class="pl-c"><span class="pl-c">--</span> SELECT * FROM person JOIN card on person.cardId = card.id;</span></pre></div>
<blockquote>
<p>注意：<code>card</code> 的整张表被连接到了右边。</p>
</blockquote>
<h4><a id="user-content-左外连接" class="anchor" aria-hidden="true" href="#左外连接"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>左外连接</h4>
<p>完整显示左边的表 ( <code>person</code> ) ，右边的表如果符合条件就显示，不符合则补 <code>NULL</code> 。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> LEFT JOIN 也叫做 LEFT OUTER JOIN，用这两种方式的查询结果是一样的。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> person <span class="pl-k">LEFT JOIN</span> card <span class="pl-k">on</span> <span class="pl-c1">person</span>.<span class="pl-c1">cardId</span> <span class="pl-k">=</span> <span class="pl-c1">card</span>.<span class="pl-c1">id</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span>
| id   | name   | cardId | id   | name      |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span>
|    <span class="pl-c1">1</span> | 张三   |      <span class="pl-c1">1</span> |    <span class="pl-c1">1</span> | 饭卡      |
|    <span class="pl-c1">2</span> | 李四   |      <span class="pl-c1">3</span> |    <span class="pl-c1">3</span> | 农行卡    |
|    <span class="pl-c1">3</span> | 王五   |      <span class="pl-c1">6</span> | <span class="pl-k">NULL</span> | <span class="pl-k">NULL</span>      |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span></pre></div>
<h4><a id="user-content-右外链接" class="anchor" aria-hidden="true" href="#右外链接"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>右外链接</h4>
<p>完整显示右边的表 ( <code>card</code> ) ，左边的表如果符合条件就显示，不符合则补 <code>NULL</code> 。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> person <span class="pl-k">RIGHT JOIN</span> card <span class="pl-k">on</span> <span class="pl-c1">person</span>.<span class="pl-c1">cardId</span> <span class="pl-k">=</span> <span class="pl-c1">card</span>.<span class="pl-c1">id</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span>
| id   | name   | cardId | id   | name      |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span>
|    <span class="pl-c1">1</span> | 张三   |      <span class="pl-c1">1</span> |    <span class="pl-c1">1</span> | 饭卡      |
|    <span class="pl-c1">2</span> | 李四   |      <span class="pl-c1">3</span> |    <span class="pl-c1">3</span> | 农行卡    |
| <span class="pl-k">NULL</span> | <span class="pl-k">NULL</span>   |   <span class="pl-k">NULL</span> |    <span class="pl-c1">2</span> | 建行卡    |
| <span class="pl-k">NULL</span> | <span class="pl-k">NULL</span>   |   <span class="pl-k">NULL</span> |    <span class="pl-c1">4</span> | 工商卡    |
| <span class="pl-k">NULL</span> | <span class="pl-k">NULL</span>   |   <span class="pl-k">NULL</span> |    <span class="pl-c1">5</span> | 邮政卡    |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span></pre></div>
<h4><a id="user-content-全外链接" class="anchor" aria-hidden="true" href="#全外链接"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>全外链接</h4>
<p>完整显示两张表的全部数据。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> MySQL 不支持这种语法的全外连接</span>
<span class="pl-c"><span class="pl-c">--</span> SELECT * FROM person FULL JOIN card on person.cardId = card.id;</span>
<span class="pl-c"><span class="pl-c">--</span> 出现错误：</span>
<span class="pl-c"><span class="pl-c">--</span> ERROR 1054 (42S22): Unknown column 'person.cardId' in 'on clause'</span>

<span class="pl-c"><span class="pl-c">--</span> MySQL全连接语法，使用 UNION 将两张表合并在一起。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> person <span class="pl-k">LEFT JOIN</span> card <span class="pl-k">on</span> <span class="pl-c1">person</span>.<span class="pl-c1">cardId</span> <span class="pl-k">=</span> <span class="pl-c1">card</span>.<span class="pl-c1">id</span>
<span class="pl-k">UNION</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> person <span class="pl-k">RIGHT JOIN</span> card <span class="pl-k">on</span> <span class="pl-c1">person</span>.<span class="pl-c1">cardId</span> <span class="pl-k">=</span> <span class="pl-c1">card</span>.<span class="pl-c1">id</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span>
| id   | name   | cardId | id   | name      |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span>
|    <span class="pl-c1">1</span> | 张三   |      <span class="pl-c1">1</span> |    <span class="pl-c1">1</span> | 饭卡      |
|    <span class="pl-c1">2</span> | 李四   |      <span class="pl-c1">3</span> |    <span class="pl-c1">3</span> | 农行卡    |
|    <span class="pl-c1">3</span> | 王五   |      <span class="pl-c1">6</span> | <span class="pl-k">NULL</span> | <span class="pl-k">NULL</span>      |
| <span class="pl-k">NULL</span> | <span class="pl-k">NULL</span>   |   <span class="pl-k">NULL</span> |    <span class="pl-c1">2</span> | 建行卡    |
| <span class="pl-k">NULL</span> | <span class="pl-k">NULL</span>   |   <span class="pl-k">NULL</span> |    <span class="pl-c1">4</span> | 工商卡    |
| <span class="pl-k">NULL</span> | <span class="pl-k">NULL</span>   |   <span class="pl-k">NULL</span> |    <span class="pl-c1">5</span> | 邮政卡    |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----+--------+--------+------+-----------+</span></pre></div>
<h2><a id="user-content-事务" class="anchor" aria-hidden="true" href="#事务"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>事务</h2>
<p>在 MySQL 中，事务其实是一个最小的不可分割的工作单元。事务能够<strong>保证一个业务的完整性</strong>。</p>
<p>比如我们的银行转账：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> a -&gt; -100</span>
<span class="pl-k">UPDATE</span> user <span class="pl-k">set</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">-</span> <span class="pl-c1">100</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>a<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> b -&gt; +100</span>
<span class="pl-k">UPDATE</span> user <span class="pl-k">set</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">+</span> <span class="pl-c1">100</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>b<span class="pl-pds">'</span></span>;</pre></div>
<p>在实际项目中，假设只有一条 SQL 语句执行成功，而另外一条执行失败了，就会出现数据前后不一致。</p>
<p>因此，在执行多条有关联 SQL 语句时，<strong>事务</strong>可能会要求这些 SQL 语句要么同时执行成功，要么就都执行失败。</p>
<h3><a id="user-content-如何控制事务---commit--rollback" class="anchor" aria-hidden="true" href="#如何控制事务---commit--rollback"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>如何控制事务 - COMMIT / ROLLBACK</h3>
<p>在 MySQL 中，事务的<strong>自动提交</strong>状态默认是开启的。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 查询事务的自动提交状态</span>
<span class="pl-k">SELECT</span> @@AUTOCOMMIT;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------+</span>
| @@AUTOCOMMIT |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------+</span>
|            <span class="pl-c1">1</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------+</span></pre></div>
<p><strong>自动提交的作用</strong>：当我们执行一条 SQL 语句的时候，其产生的效果就会立即体现出来，且不能<strong>回滚</strong>。</p>
<p>什么是回滚？举个例子：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">CREATE</span> <span class="pl-k">DATABASE</span> <span class="pl-en">bank</span>;

USE bank;

<span class="pl-k">CREATE</span> <span class="pl-k">TABLE</span> <span class="pl-en">user</span> (
    id <span class="pl-k">INT</span> <span class="pl-k">PRIMARY KEY</span>,
    name <span class="pl-k">VARCHAR</span>(<span class="pl-c1">20</span>),
    <span class="pl-k">money</span> <span class="pl-k">INT</span>
);

<span class="pl-k">INSERT INTO</span> user <span class="pl-k">VALUES</span> (<span class="pl-c1">1</span>, <span class="pl-s"><span class="pl-pds">'</span>a<span class="pl-pds">'</span></span>, <span class="pl-c1">1000</span>);

<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span></pre></div>
<p>可以看到，在执行插入语句后数据立刻生效，原因是 MySQL 中的事务自动将它<strong>提交</strong>到了数据库中。那么所谓<strong>回滚</strong>的意思就是，撤销执行过的所有 SQL 语句，使其回滚到<strong>最后一次提交</strong>数据时的状态。</p>
<p>在 MySQL 中使用 <code>ROLLBACK</code> 执行回滚：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 回滚到最后一次提交</span>
<span class="pl-k">ROLLBACK</span>;

<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span></pre></div>
<p>由于所有执行过的 SQL 语句都已经被提交过了，所以数据并没有发生回滚。那如何让数据可以发生回滚？</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 关闭自动提交</span>
<span class="pl-k">SET</span> AUTOCOMMIT <span class="pl-k">=</span> <span class="pl-c1">0</span>;

<span class="pl-c"><span class="pl-c">--</span> 查询自动提交状态</span>
<span class="pl-k">SELECT</span> @@AUTOCOMMIT;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------+</span>
| @@AUTOCOMMIT |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------+</span>
|            <span class="pl-c1">0</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------+</span></pre></div>
<p>将自动提交关闭后，测试数据回滚：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">INSERT INTO</span> user <span class="pl-k">VALUES</span> (<span class="pl-c1">2</span>, <span class="pl-s"><span class="pl-pds">'</span>b<span class="pl-pds">'</span></span>, <span class="pl-c1">1000</span>);

<span class="pl-c"><span class="pl-c">--</span> 关闭 AUTOCOMMIT 后，数据的变化是在一张虚拟的临时数据表中展示，</span>
<span class="pl-c"><span class="pl-c">--</span> 发生变化的数据并没有真正插入到数据表中。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">2</span> | b    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>

<span class="pl-c"><span class="pl-c">--</span> 数据表中的真实数据其实还是：</span>
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>

<span class="pl-c"><span class="pl-c">--</span> 由于数据还没有真正提交，可以使用回滚</span>
<span class="pl-k">ROLLBACK</span>;

<span class="pl-c"><span class="pl-c">--</span> 再次查询</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span></pre></div>
<p>那如何将虚拟的数据真正提交到数据库中？使用 <code>COMMIT</code> :</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">INSERT INTO</span> user <span class="pl-k">VALUES</span> (<span class="pl-c1">2</span>, <span class="pl-s"><span class="pl-pds">'</span>b<span class="pl-pds">'</span></span>, <span class="pl-c1">1000</span>);
<span class="pl-c"><span class="pl-c">--</span> 手动提交数据（持久性），</span>
<span class="pl-c"><span class="pl-c">--</span> 将数据真正提交到数据库中，执行后不能再回滚提交过的数据。</span>
<span class="pl-k">COMMIT</span>;

<span class="pl-c"><span class="pl-c">--</span> 提交后测试回滚</span>
<span class="pl-k">ROLLBACK</span>;

<span class="pl-c"><span class="pl-c">--</span> 再次查询（回滚无效了）</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">2</span> | b    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span></pre></div>
<blockquote>
<p><strong>总结</strong></p>
<ol>
<li>
<p><strong>自动提交</strong></p>
<ul>
<li>
<p>查看自动提交状态：<code>SELECT @@AUTOCOMMIT</code> ；</p>
</li>
<li>
<p>设置自动提交状态：<code>SET AUTOCOMMIT = 0</code> 。</p>
</li>
</ul>
</li>
<li>
<p><strong>手动提交</strong></p>
<p><code>@@AUTOCOMMIT = 0</code> 时，使用 <code>COMMIT</code> 命令提交事务。</p>
</li>
<li>
<p><strong>事务回滚</strong></p>
<p><code>@@AUTOCOMMIT = 0</code> 时，使用 <code>ROLLBACK</code> 命令回滚事务。</p>
</li>
</ol>
</blockquote>
<p><strong>事务的实际应用</strong>，让我们再回到银行转账项目：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 转账</span>
<span class="pl-k">UPDATE</span> user <span class="pl-k">set</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">-</span> <span class="pl-c1">100</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>a<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> 到账</span>
<span class="pl-k">UPDATE</span> user <span class="pl-k">set</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">+</span> <span class="pl-c1">100</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>b<span class="pl-pds">'</span></span>;

<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b    |  <span class="pl-c1">1100</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span></pre></div>
<p>这时假设在转账时发生了意外，就可以使用 <code>ROLLBACK</code> 回滚到最后一次提交的状态：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 假设转账发生了意外，需要回滚。</span>
<span class="pl-k">ROLLBACK</span>;

<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">2</span> | b    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span></pre></div>
<p>这时我们又回到了发生意外之前的状态，也就是说，事务给我们提供了一个可以反悔的机会。假设数据没有发生意外，这时可以手动将数据真正提交到数据表中：<code>COMMIT</code> 。</p>
<h3><a id="user-content-手动开启事务---begin--start-transaction" class="anchor" aria-hidden="true" href="#手动开启事务---begin--start-transaction"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>手动开启事务 - BEGIN / START TRANSACTION</h3>
<p>事务的默认提交被开启 ( <code>@@AUTOCOMMIT = 1</code> ) 后，此时就不能使用事务回滚了。但是我们还可以手动开启一个事务处理事件，使其可以发生回滚：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 使用 BEGIN 或者 START TRANSACTION 手动开启一个事务</span>
<span class="pl-c"><span class="pl-c">--</span> START TRANSACTION;</span>
<span class="pl-k">BEGIN</span>;
<span class="pl-k">UPDATE</span> user <span class="pl-k">set</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">-</span> <span class="pl-c1">100</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>a<span class="pl-pds">'</span></span>;
<span class="pl-k">UPDATE</span> user <span class="pl-k">set</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">+</span> <span class="pl-c1">100</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>b<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> 由于手动开启的事务没有开启自动提交，</span>
<span class="pl-c"><span class="pl-c">--</span> 此时发生变化的数据仍然是被保存在一张临时表中。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b    |  <span class="pl-c1">1100</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>

<span class="pl-c"><span class="pl-c">--</span> 测试回滚</span>
<span class="pl-k">ROLLBACK</span>;

<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">2</span> | b    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span></pre></div>
<p>仍然使用 <code>COMMIT</code> 提交数据，提交后无法再发生本次事务的回滚。</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">BEGIN</span>;
<span class="pl-k">UPDATE</span> user <span class="pl-k">set</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">-</span> <span class="pl-c1">100</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>a<span class="pl-pds">'</span></span>;
<span class="pl-k">UPDATE</span> user <span class="pl-k">set</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">+</span> <span class="pl-c1">100</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>b<span class="pl-pds">'</span></span>;

<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
| id | name | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>
|  <span class="pl-c1">1</span> | a    |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b    |  <span class="pl-c1">1100</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+------+-------+</span>

<span class="pl-c"><span class="pl-c">--</span> 提交数据</span>
<span class="pl-k">COMMIT</span>;

<span class="pl-c"><span class="pl-c">--</span> 测试回滚（无效，因为表的数据已经被提交）</span>
<span class="pl-k">ROLLBACK</span>;</pre></div>
<h3><a id="user-content-事务的-acid-特征与使用" class="anchor" aria-hidden="true" href="#事务的-acid-特征与使用"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>事务的 ACID 特征与使用</h3>
<p><strong>事务的四大特征：</strong></p>
<ul>
<li><strong>A 原子性</strong>：事务是最小的单位，不可以再分割；</li>
<li><strong>C 一致性</strong>：要求同一事务中的 SQL 语句，必须保证同时成功或者失败；</li>
<li><strong>I 隔离性</strong>：事务1 和 事务2 之间是具有隔离性的；</li>
<li><strong>D 持久性</strong>：事务一旦结束 ( <code>COMMIT</code> ) ，就不可以再返回了 ( <code>ROLLBACK</code> ) 。</li>
</ul>
<h3><a id="user-content-事务的隔离性" class="anchor" aria-hidden="true" href="#事务的隔离性"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>事务的隔离性</h3>
<p><strong>事务的隔离性可分为四种 ( 性能从低到高 )</strong> ：</p>
<ol>
<li>
<p><strong>READ UNCOMMITTED ( 读取未提交 )</strong></p>
<p>如果有多个事务，那么任意事务都可以看见其他事务的<strong>未提交数据</strong>。</p>
</li>
<li>
<p><strong>READ COMMITTED ( 读取已提交 )</strong></p>
<p>只能读取到其他事务<strong>已经提交的数据</strong>。</p>
</li>
<li>
<p><strong>REPEATABLE READ ( 可被重复读 )</strong></p>
<p>如果有多个连接都开启了事务，那么事务之间不能共享数据记录，否则只能共享已提交的记录。</p>
</li>
<li>
<p><strong>SERIALIZABLE ( 串行化 )</strong></p>
<p>所有的事务都会按照<strong>固定顺序执行</strong>，执行完一个事务后再继续执行下一个事务的<strong>写入操作</strong>。</p>
</li>
</ol>
<p>查看当前数据库的默认隔离级别：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> MySQL 8.x, GLOBAL 表示系统级别，不加表示会话级别。</span>
<span class="pl-k">SELECT</span> @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span>;
<span class="pl-k">SELECT</span> @@TRANSACTION_ISOLATION;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| REPEATABLE<span class="pl-k">-</span>READ                | <span class="pl-c"><span class="pl-c">--</span> MySQL的默认隔离级别，可以重复读。</span>
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>

<span class="pl-c"><span class="pl-c">--</span> MySQL 5.x</span>
<span class="pl-k">SELECT</span> @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TX_ISOLATION</span>;
<span class="pl-k">SELECT</span> @@TX_ISOLATION;</pre></div>
<p>修改隔离级别：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 设置系统隔离级别，LEVEL 后面表示要设置的隔离级别 (READ UNCOMMITTED)。</span>
<span class="pl-k">SET</span> GLOBAL TRANSACTION ISOLATION LEVEL READ UNCOMMITTED;

<span class="pl-c"><span class="pl-c">--</span> 查询系统隔离级别，发现已经被修改。</span>
<span class="pl-k">SELECT</span> @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| READ<span class="pl-k">-</span>UNCOMMITTED               |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span></pre></div>
<h4><a id="user-content-脏读" class="anchor" aria-hidden="true" href="#脏读"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>脏读</h4>
<p>测试 <strong>READ UNCOMMITTED ( 读取未提交 )</strong> 的隔离性：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">INSERT INTO</span> user <span class="pl-k">VALUES</span> (<span class="pl-c1">3</span>, <span class="pl-s"><span class="pl-pds">'</span>小明<span class="pl-pds">'</span></span>, <span class="pl-c1">1000</span>);
<span class="pl-k">INSERT INTO</span> user <span class="pl-k">VALUES</span> (<span class="pl-c1">4</span>, <span class="pl-s"><span class="pl-pds">'</span>淘宝店<span class="pl-pds">'</span></span>, <span class="pl-c1">1000</span>);

<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
| id | name      | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
|  <span class="pl-c1">1</span> | a         |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b         |  <span class="pl-c1">1100</span> |
|  <span class="pl-c1">3</span> | 小明      |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">4</span> | 淘宝店    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>

<span class="pl-c"><span class="pl-c">--</span> 开启一个事务操作数据</span>
<span class="pl-c"><span class="pl-c">--</span> 假设小明在淘宝店买了一双800块钱的鞋子：</span>
<span class="pl-k">START TRANSACTION</span>;
<span class="pl-k">UPDATE</span> user <span class="pl-k">SET</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">-</span> <span class="pl-c1">800</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>小明<span class="pl-pds">'</span></span>;
<span class="pl-k">UPDATE</span> user <span class="pl-k">SET</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">+</span> <span class="pl-c1">800</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>淘宝店<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> 然后淘宝店在另一方查询结果，发现钱已到账。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
| id | name      | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
|  <span class="pl-c1">1</span> | a         |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b         |  <span class="pl-c1">1100</span> |
|  <span class="pl-c1">3</span> | 小明      |   <span class="pl-c1">200</span> |
|  <span class="pl-c1">4</span> | 淘宝店    |  <span class="pl-c1">1800</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span></pre></div>
<p>由于小明的转账是在新开启的事务上进行操作的，而该操作的结果是可以被其他事务（另一方的淘宝店）看见的，因此淘宝店的查询结果是正确的，淘宝店确认到账。但就在这时，如果小明在它所处的事务上又执行了 <code>ROLLBACK</code> 命令，会发生什么？</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 小明所处的事务</span>
<span class="pl-k">ROLLBACK</span>;

<span class="pl-c"><span class="pl-c">--</span> 此时无论对方是谁，如果再去查询结果就会发现：</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
| id | name      | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
|  <span class="pl-c1">1</span> | a         |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b         |  <span class="pl-c1">1100</span> |
|  <span class="pl-c1">3</span> | 小明      |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">4</span> | 淘宝店    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span></pre></div>
<p>这就是所谓的<strong>脏读</strong>，一个事务读取到另外一个事务还未提交的数据。这在实际开发中是不允许出现的。</p>
<h4><a id="user-content-读取已提交" class="anchor" aria-hidden="true" href="#读取已提交"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>读取已提交</h4>
<p>把隔离级别设置为 <strong>READ COMMITTED</strong> ：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SET</span> GLOBAL TRANSACTION ISOLATION LEVEL READ COMMITTED;
<span class="pl-k">SELECT</span> @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| READ<span class="pl-k">-</span>COMMITTED                 |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span></pre></div>
<p>这样，再有新的事务连接进来时，它们就只能查询到已经提交过的事务数据了。但是对于当前事务来说，它们看到的还是未提交的数据，例如：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 正在操作数据事务（当前事务）</span>
<span class="pl-k">START TRANSACTION</span>;
<span class="pl-k">UPDATE</span> user <span class="pl-k">SET</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">-</span> <span class="pl-c1">800</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>小明<span class="pl-pds">'</span></span>;
<span class="pl-k">UPDATE</span> user <span class="pl-k">SET</span> <span class="pl-k">money</span> <span class="pl-k">=</span> <span class="pl-k">money</span> <span class="pl-k">+</span> <span class="pl-c1">800</span> <span class="pl-k">WHERE</span> name <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>淘宝店<span class="pl-pds">'</span></span>;

<span class="pl-c"><span class="pl-c">--</span> 虽然隔离级别被设置为了 READ COMMITTED，但在当前事务中，</span>
<span class="pl-c"><span class="pl-c">--</span> 它看到的仍然是数据表中临时改变数据，而不是真正提交过的数据。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
| id | name      | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
|  <span class="pl-c1">1</span> | a         |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b         |  <span class="pl-c1">1100</span> |
|  <span class="pl-c1">3</span> | 小明      |   <span class="pl-c1">200</span> |
|  <span class="pl-c1">4</span> | 淘宝店    |  <span class="pl-c1">1800</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>


<span class="pl-c"><span class="pl-c">--</span> 假设此时在远程开启了一个新事务，连接到数据库。</span>
$ mysql <span class="pl-k">-</span>u root <span class="pl-k">-</span>p12345612

<span class="pl-c"><span class="pl-c">--</span> 此时远程连接查询到的数据只能是已经提交过的</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
| id | name      | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
|  <span class="pl-c1">1</span> | a         |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b         |  <span class="pl-c1">1100</span> |
|  <span class="pl-c1">3</span> | 小明      |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">4</span> | 淘宝店    |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span></pre></div>
<p>但是这样还有问题，那就是假设一个事务在操作数据时，其他事务干扰了这个事务的数据。例如：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 小张在查询数据的时候发现：</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
| id | name      | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
|  <span class="pl-c1">1</span> | a         |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b         |  <span class="pl-c1">1100</span> |
|  <span class="pl-c1">3</span> | 小明      |   <span class="pl-c1">200</span> |
|  <span class="pl-c1">4</span> | 淘宝店    |  <span class="pl-c1">1800</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>

<span class="pl-c"><span class="pl-c">--</span> 在小张求表的 money 平均值之前，小王做了一个操作：</span>
<span class="pl-k">START TRANSACTION</span>;
<span class="pl-k">INSERT INTO</span> user <span class="pl-k">VALUES</span> (<span class="pl-c1">5</span>, <span class="pl-s"><span class="pl-pds">'</span>c<span class="pl-pds">'</span></span>, <span class="pl-c1">100</span>);
<span class="pl-k">COMMIT</span>;

<span class="pl-c"><span class="pl-c">--</span> 此时表的真实数据是：</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
| id | name      | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
|  <span class="pl-c1">1</span> | a         |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b         |  <span class="pl-c1">1100</span> |
|  <span class="pl-c1">3</span> | 小明      |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">4</span> | 淘宝店    |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">5</span> | c         |   <span class="pl-c1">100</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>

<span class="pl-c"><span class="pl-c">--</span> 这时小张再求平均值的时候，就会出现计算不相符合的情况：</span>
<span class="pl-k">SELECT</span> <span class="pl-c1">AVG</span>(<span class="pl-k">money</span>) <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----------+</span>
| <span class="pl-c1">AVG</span>(<span class="pl-k">money</span>) |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----------+</span>
|  <span class="pl-c1">820</span>.<span class="pl-c1">0000</span>  |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>----------+</span></pre></div>
<p>虽然 <strong>READ COMMITTED</strong> 让我们只能读取到其他事务已经提交的数据，但还是会出现问题，就是<strong>在读取同一个表的数据时，可能会发生前后不一致的情况。<strong>这被称为</strong>不可重复读现象 ( READ COMMITTED )</strong> 。</p>
<h4><a id="user-content-幻读" class="anchor" aria-hidden="true" href="#幻读"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>幻读</h4>
<p>将隔离级别设置为 <strong>REPEATABLE READ ( 可被重复读取 )</strong> :</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SET</span> GLOBAL TRANSACTION ISOLATION LEVEL REPEATABLE READ;
<span class="pl-k">SELECT</span> @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| REPEATABLE<span class="pl-k">-</span>READ                |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span></pre></div>
<p>测试 <strong>REPEATABLE READ</strong> ，假设在两个不同的连接上分别执行 <code>START TRANSACTION</code> :</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 小张 - 成都</span>
<span class="pl-k">START TRANSACTION</span>;
<span class="pl-k">INSERT INTO</span> user <span class="pl-k">VALUES</span> (<span class="pl-c1">6</span>, <span class="pl-s"><span class="pl-pds">'</span>d<span class="pl-pds">'</span></span>, <span class="pl-c1">1000</span>);

<span class="pl-c"><span class="pl-c">--</span> 小王 - 北京</span>
<span class="pl-k">START TRANSACTION</span>;

<span class="pl-c"><span class="pl-c">--</span> 小张 - 成都</span>
<span class="pl-k">COMMIT</span>;</pre></div>
<p>当前事务开启后，没提交之前，查询不到，提交后可以被查询到。但是，在提交之前其他事务被开启了，那么在这条事务线上，就不会查询到当前有操作事务的连接。相当于开辟出一条单独的线程。</p>
<p>无论小张是否执行过 <code>COMMIT</code> ，在小王这边，都不会查询到小张的事务记录，而是只会查询到自己所处事务的记录：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
| id | name      | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
|  <span class="pl-c1">1</span> | a         |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b         |  <span class="pl-c1">1100</span> |
|  <span class="pl-c1">3</span> | 小明      |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">4</span> | 淘宝店    |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">5</span> | c         |   <span class="pl-c1">100</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span></pre></div>
<p>这是<strong>因为小王在此之前开启了一个新的事务 ( <code>START TRANSACTION</code> ) <strong>，那么</strong>在他的这条新事务的线上，跟其他事务是没有联系的</strong>，也就是说，此时如果其他事务正在操作数据，它是不知道的。</p>
<p>然而事实是，在真实的数据表中，小张已经插入了一条数据。但是小王此时并不知道，也插入了同一条数据，会发生什么呢？</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">INSERT INTO</span> user <span class="pl-k">VALUES</span> (<span class="pl-c1">6</span>, <span class="pl-s"><span class="pl-pds">'</span>d<span class="pl-pds">'</span></span>, <span class="pl-c1">1000</span>);
<span class="pl-c"><span class="pl-c">--</span> ERROR 1062 (23000): Duplicate entry '6' for key 'PRIMARY'</span></pre></div>
<p>报错了，操作被告知已存在主键为 <code>6</code> 的字段。这种现象也被称为<strong>幻读，一个事务提交的数据，不能被其他事务读取到</strong>。</p>
<h4><a id="user-content-串行化" class="anchor" aria-hidden="true" href="#串行化"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>串行化</h4>
<p>顾名思义，就是所有事务的<strong>写入操作</strong>全都是串行化的。什么意思？把隔离级别修改成 <strong>SERIALIZABLE</strong> :</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-k">SET</span> GLOBAL TRANSACTION ISOLATION LEVEL SERIALIZABLE;
<span class="pl-k">SELECT</span> @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span>;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| @@<span class="pl-c1">GLOBAL</span>.<span class="pl-c1">TRANSACTION_ISOLATION</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span>
| SERIALIZABLE                   |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>------------------------------+</span></pre></div>
<p>还是拿小张和小王来举例：</p>
<div class="highlight highlight-source-sql"><pre><span class="pl-c"><span class="pl-c">--</span> 小张 - 成都</span>
<span class="pl-k">START TRANSACTION</span>;

<span class="pl-c"><span class="pl-c">--</span> 小王 - 北京</span>
<span class="pl-k">START TRANSACTION</span>;

<span class="pl-c"><span class="pl-c">--</span> 开启事务之前先查询表，准备操作数据。</span>
<span class="pl-k">SELECT</span> <span class="pl-k">*</span> <span class="pl-k">FROM</span> user;
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
| id | name      | <span class="pl-k">money</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>
|  <span class="pl-c1">1</span> | a         |   <span class="pl-c1">900</span> |
|  <span class="pl-c1">2</span> | b         |  <span class="pl-c1">1100</span> |
|  <span class="pl-c1">3</span> | 小明      |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">4</span> | 淘宝店    |  <span class="pl-c1">1000</span> |
|  <span class="pl-c1">5</span> | c         |   <span class="pl-c1">100</span> |
|  <span class="pl-c1">6</span> | d         |  <span class="pl-c1">1000</span> |
<span class="pl-k">+</span><span class="pl-c"><span class="pl-c">--</span>--+-----------+-------+</span>

<span class="pl-c"><span class="pl-c">--</span> 发现没有 7 号王小花，于是插入一条数据：</span>
<span class="pl-k">INSERT INTO</span> user <span class="pl-k">VALUES</span> (<span class="pl-c1">7</span>, <span class="pl-s"><span class="pl-pds">'</span>王小花<span class="pl-pds">'</span></span>, <span class="pl-c1">1000</span>);</pre></div>
<p>此时会发生什么呢？由于现在的隔离级别是 <strong>SERIALIZABLE ( 串行化 )</strong> ，串行化的意思就是：假设把所有的事务都放在一个串行的队列中，那么所有的事务都会按照<strong>固定顺序执行</strong>，执行完一个事务后再继续执行下一个事务的<strong>写入操作</strong> ( <strong>这意味着队列中同时只能执行一个事务的写入操作</strong> ) 。</p>
<p>根据这个解释，小王在插入数据时，会出现等待状态，直到小张执行 <code>COMMIT</code> 结束它所处的事务，或者出现等待超时。</p>
</article>
  </div>

    </div>

  

  <details class="details-reset details-overlay details-overlay-dark">
    <summary data-hotkey="l" aria-label="Jump to line"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast linejump" aria-label="Jump to line">
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-jump-to-line-form Box-body d-flex" action="" accept-charset="UTF-8" method="get">
        <input class="form-control flex-auto mr-3 linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
        <button type="submit" class="btn" data-close-dialog>Go</button>
</form>    </details-dialog>
  </details>



  </div>
</div>

    </main>
  </div>
  

  </div>

        
<div class="footer container-lg width-full p-responsive" role="contentinfo">
  <div class="position-relative d-flex flex-row-reverse flex-lg-row flex-wrap flex-lg-nowrap flex-justify-center flex-lg-justify-between pt-6 pb-2 mt-6 f6 text-gray border-top border-gray-light ">
    <ul class="list-style-none d-flex flex-wrap col-12 col-lg-5 flex-justify-center flex-lg-justify-between mb-2 mb-lg-0">
      <li class="mr-3 mr-lg-0">&copy; 2020 GitHub, Inc.</li>
        <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to terms, text:terms" href="https://github.com/site/terms">Terms</a></li>
        <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to privacy, text:privacy" href="https://github.com/site/privacy">Privacy</a></li>
        <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to security, text:security" href="https://github.com/security">Security</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://githubstatus.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a data-ga-click="Footer, go to help, text:help" href="https://help.github.com">Help</a></li>

    </ul>

    <a aria-label="Homepage" title="GitHub" class="footer-octicon d-none d-lg-block mx-lg-4" href="https://github.com">
      <svg height="24" class="octicon octicon-mark-github" viewBox="0 0 16 16" version="1.1" width="24" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"/></svg>
</a>
   <ul class="list-style-none d-flex flex-wrap col-12 col-lg-5 flex-justify-center flex-lg-justify-between mb-2 mb-lg-0">
        <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to contact, text:contact" href="https://github.com/contact">Contact GitHub</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://github.com/pricing" data-ga-click="Footer, go to Pricing, text:Pricing">Pricing</a></li>
      <li class="mr-3 mr-lg-0"><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li class="mr-3 mr-lg-0"><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://github.blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a data-ga-click="Footer, go to about, text:about" href="https://github.com/about">About</a></li>
    </ul>
  </div>
  <div class="d-flex flex-justify-center pb-6">
    <span class="f6 text-gray-light"></span>
  </div>
</div>



  <div id="ajax-error-message" class="ajax-error-message flash flash-error">
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 000 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 00.01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <button type="button" class="flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
    </button>
    You can’t perform that action at this time.
  </div>


    <script crossorigin="anonymous" async="async" integrity="sha512-o4vS4IKrjdy/HD+xr2+VhO6DxQmj5jikhHbEGrd8+JGhpmIOxRrpT1Qo5k3IhKimm8VXIu3pyYejLtOAkm+OsQ==" type="application/javascript" id="js-conditional-compat" data-src="https://github.githubassets.com/assets/compat-bootstrap-a38bd2e0.js"></script>
    <script crossorigin="anonymous" integrity="sha512-2GtXiukHeT1/Kt5UHrVa2iMiBF1fCLQILWG0UKazKtQXjLZpcurZ6AXlkiTZFUeEtVWjoV8LvyppgPp9rkQMUA==" type="application/javascript" src="https://github.githubassets.com/assets/environment-bootstrap-d86b578a.js"></script>
    <script crossorigin="anonymous" async="async" integrity="sha512-b/eiTgUmQXvFSyXcioklOO+SOVe85tsZw2OyDiixI8/rzI71a+4eh2LljU/7co1ItCsS9iSI+wp+2BB0SMfK8A==" type="application/javascript" src="https://github.githubassets.com/assets/vendor-6ff7a24e.js"></script>
    <script crossorigin="anonymous" async="async" integrity="sha512-Fc+yj6iF9vKV0zGUXRaexKGT7ZOMPeTR3MNd54+fs1PGJ+/tK66NSmobzxslmB2J+HXnBHIUaCm3ww3GNW+o8g==" type="application/javascript" src="https://github.githubassets.com/assets/frameworks-15cfb28f.js"></script>
    
    <script crossorigin="anonymous" async="async" integrity="sha512-nQeS+KxdgRVLSjgfF9qkWRWBLrtrxpcNAZVK5KPcZtDwxe6h7AJqUWc3U5U9xMfZvbkwecgoTeUjxGBlEBfRzA==" type="application/javascript" src="https://github.githubassets.com/assets/github-bootstrap-9d0792f8.js"></script>
    
    
    
  <div class="js-stale-session-flash flash flash-warn flash-banner" hidden
    >
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 000 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 00.01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <span class="js-stale-session-flash-signed-in" hidden>You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="js-stale-session-flash-signed-out" hidden>You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
  <template id="site-details-dialog">
  <details class="details-reset details-overlay details-overlay-dark lh-default text-gray-dark hx_rsm" open>
    <summary role="button" aria-label="Close dialog"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast hx_rsm-dialog hx_rsm-modal">
      <button class="Box-btn-octicon m-0 btn-octicon position-absolute right-0 top-0" type="button" aria-label="Close dialog" data-close-dialog>
        <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
      </button>
      <div class="octocat-spinner my-6 js-details-dialog-spinner"></div>
    </details-dialog>
  </details>
</template>

  <div class="Popover js-hovercard-content position-absolute" style="display: none; outline: none;" tabindex="0">
  <div class="Popover-message Popover-message--bottom-left Popover-message--large Box box-shadow-large" style="width:360px;">
  </div>
</div>

  <div aria-live="polite" class="js-global-screen-reader-notice sr-only"></div>

  </body>
</html>

