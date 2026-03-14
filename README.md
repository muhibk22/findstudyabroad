# Study Abroad Consultant Platform

## Project Structure

```
study-abroad-platform/
├── src/
│   ├── app/
│   │   ├── (public)/                   # Student-facing public pages
│   │   │   ├── layout.tsx
│   │   │   ├── page.tsx                # Homepage
│   │   │   ├── blogs/
│   │   │   │   ├── page.tsx
│   │   │   │   └── [slug]/
│   │   │   │       └── page.tsx
│   │   │   ├── news/
│   │   │   │   ├── page.tsx
│   │   │   │   └── [slug]/
│   │   │   │       └── page.tsx
│   │   │   ├── scholarships/
│   │   │   │   └── page.tsx
│   │   │   └── apply/
│   │   │       └── page.tsx            # Lead submission form
│   │   │
│   │   ├── admin/                      # Consultant dashboard (xyz.com/admin)
│   │   │   ├── layout.tsx
│   │   │   ├── page.tsx
│   │   │   ├── leads/
│   │   │   │   ├── page.tsx
│   │   │   │   └── [id]/
│   │   │   │       └── page.tsx
│   │   │   ├── blogs/
│   │   │   │   ├── page.tsx
│   │   │   │   ├── new/
│   │   │   │   │   └── page.tsx
│   │   │   │   └── [id]/edit/
│   │   │   │       └── page.tsx
│   │   │   ├── news/
│   │   │   │   ├── page.tsx
│   │   │   │   ├── new/
│   │   │   │   │   └── page.tsx
│   │   │   │   └── [id]/edit/
│   │   │   │       └── page.tsx
│   │   │   ├── ads/
│   │   │   │   ├── page.tsx
│   │   │   │   └── new/
│   │   │   │       └── page.tsx
│   │   │   └── profile/
│   │   │       └── page.tsx
│   │   │
│   │   ├── (admin-panel)/              # Platform admin dashboard (admin.xyz.com)
│   │   │   ├── layout.tsx
│   │   │   ├── page.tsx                # Analytics overview
│   │   │   ├── leads/
│   │   │   │   ├── page.tsx            # Approve / reject leads
│   │   │   │   └── [id]/
│   │   │   │       └── page.tsx
│   │   │   ├── consultants/
│   │   │   │   ├── page.tsx
│   │   │   │   └── [id]/
│   │   │   │       └── page.tsx
│   │   │   ├── cities/
│   │   │   │   ├── page.tsx
│   │   │   │   └── new/
│   │   │   │       └── page.tsx
│   │   │   ├── content/
│   │   │   │   ├── blogs/
│   │   │   │   │   └── page.tsx
│   │   │   │   └── news/
│   │   │   │       └── page.tsx
│   │   │   └── ads/
│   │   │       ├── page.tsx
│   │   │       └── [id]/
│   │   │           └── page.tsx
│   │   │
│   │   └── api/
│   │       ├── auth/
│   │       │   └── [...nextauth]/
│   │       │       └── route.ts
│   │       ├── leads/
│   │       │   ├── route.ts
│   │       │   └── [id]/
│   │       │       └── route.ts
│   │       ├── consultants/
│   │       │   ├── route.ts
│   │       │   └── [id]/
│   │       │       └── route.ts
│   │       ├── cities/
│   │       │   └── route.ts
│   │       ├── blogs/
│   │       │   ├── route.ts
│   │       │   └── [id]/
│   │       │       └── route.ts
│   │       ├── news/
│   │       │   ├── route.ts
│   │       │   └── [id]/
│   │       │       └── route.ts
│   │       ├── scholarships/
│   │       │   └── route.ts
│   │       └── ads/
│   │           ├── route.ts
│   │           └── [id]/
│   │               └── route.ts
│   │
│   ├── components/
│   │   ├── ui/
│   │   ├── public/
│   │   ├── consultant/
│   │   └── admin-panel/
│   │
│   ├── lib/
│   │   ├── db.ts
│   │   ├── auth.ts
│   │   └── utils.ts
│   │
│   ├── models/
│   │   ├── Lead.ts
│   │   ├── Consultant.ts
│   │   ├── City.ts
│   │   ├── Blog.ts
│   │   ├── News.ts
│   │   ├── Scholarship.ts
│   │   └── Ad.ts
│   │
│   ├── middleware.ts
│   └── types/
│       └── index.ts
│
├── public/
├── .env.local
├── next.config.ts
├── tailwind.config.ts
└── package.json
```

---

## Environment Variables

```env
# MongoDB
MONGODB_URI=

# NextAuth
NEXTAUTH_SECRET=your_secret_here
NEXTAUTH_URL=http://localhost:3000

# Cloudinary
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret


```