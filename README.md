# Metaversus Project
Build and Deploy a Modern Next 13 Website With Framer Motion & Tailwind CSS

## Getting Started

Điểm khác biệt với Next phiên bản cũ hơn:
- Cách tổ chức folder gọn gàng hơn: 
==> Thư mục app để router, cũng như chứa các trang đặc biệt của project. Tham khảo File Conventions (https://beta.nextjs.org/docs/api-reference/file-conventions/layout)

==> Thư mục pages giờ đây chỉ còn chứa api

==> Cập nhật thêm ...

**Điểm khác biệt lớn nhất:**
Server and Client Components
```
All components inside the app directory are React Server Components by default, including special files and colocated components. This allows you to automatically adopt Server Components with no extra work, and achieve great performance out of the box
```
How to transform the server side component to a client-side component
=> A component becomes a Client Component when using the "use client" directive at the top of the file (before any imports).
```
What do you need to do?                                                          Server Component                               Client Component
---
Fetch data. Learn more.	                                                                ✅	                                         ⚠️
---
Access backend resources (directly)	                                                    ✅	                                         ❌
---
Keep sensitive information on the server (access tokens, API keys, etc)	                ✅	                                         ❌
---
Keep large dependencies on the server / Reduce client-side JavaScript	                ✅	                                         ❌
---
Add interactivity and event listeners (onClick(), onChange(), etc)	                    ❌	                                         ✅
---
Use State and Lifecycle Effects (useState(), useReducer(), useEffect(), etc)	        ❌	                                         ✅
---
Use browser-only APIs	                                                                ❌	                                         ✅
---
Use custom hooks that depend on state, effects, or browser-only APIs	                ❌	                                         ✅
---
Use React Class components	                                                            ❌	                                         ✅
---
```

## Deploy on Vercel
