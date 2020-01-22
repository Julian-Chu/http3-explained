# پروتکل QUIC چطور کار می‌کند

بدون توضیح دقیق ریز و درشت‌ها (بیت‌ و بایت‌ها) این بخش نحوه کارکردِ قطعاتِ اساسیِ سازنده‌یِ پروتکلِ انتقالِ QUIC را شرح می‌دهد. اگر شما قصد دارید تا پشته‌ی QUIC خودتان را پیاده‌سازی کنید، این تشریح‌ بایست یک فهم و دید کلی به شما بدهد، اما برای تمامی جزئیات، به پیش ‌نویس‌ها و RFC های کارگروه مهندسی اینترنت (IETF) رجوع نمایید.

۱. یک [اتصال](quic-connections.md) برقرار نمایید

۲. ... که شامل [امنیت TLS](quic-tls.md) باشد

۳. سپس از [جریان‌ها](quic-streams.md) استفاده نمایید