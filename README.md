import { BlogPosts } from 'app/components/posts'

export default function Page() {
  return (
    <section style={{ backgroundColor: '#FAFAFA', minHeight: '100vh', padding: '2rem 1rem' }}>
      {/* Brand Header & Logo Section */}
      <div style={{ textAlign: 'center', marginBottom: '3rem' }}>
        <h1 className="text-4xl font-semibold tracking-tighter" style={{ color: '#111827', marginBottom: '0.5rem' }}>
          MedEasyLearn
        </h1>
        <p style={{ color: '#007A87', fontWeight: '500', letterSpacing: '0.05em', textTransform: 'uppercase', fontSize: '0.875rem' }}>
          Making Medical Knowledge Simple
        </p>
      </div>

      {/* About Dr. Arif Introduction */}
      <div style={{ maxWidth: '650px', margin: '0 auto 4rem auto', color: '#111827' }}>
        <h2 className="text-2xl font-medium tracking-tight" style={{ marginBottom: '1rem' }}>
          Hi, I'm Dr. Mohammad Arif
        </h2>
        <p className="prose prose-neutral dark:prose-invert" style={{ lineHeight: '1.75', marginBottom: '1.5rem' }}>
          Welcome to my digital workspace. As a medical professional, my mission is to break down complex clinical concepts, high-yield exam topics, and medical guidelines into simple, actionable daily insights for medical students and healthcare professionals worldwide.
        </p>

        {/* Social Media Link Button */}
        <a 
          href="https://instagram.com" 
          target="_blank" 
          rel="noopener noreferrer"
          style={{ 
            display: 'inline-flex', 
            backgroundColor: '#111827', 
            color: '#FFFFFF', 
            padding: '0.5rem 1rem', 
            borderRadius: '0.375rem', 
            fontWeight: '500',
            fontSize: '0.875rem',
            textDecoration: 'none'
          }}
        >
          Follow Daily on Instagram →
        </a>
      </div>

      {/* Daily Medical Blog Section */}
      <div style={{ maxWidth: '650px', margin: '0 auto' }}>
        <h3 className="text-xl font-medium tracking-tight" style={{ color: '#111827', marginBottom: '1.5rem', borderBottom: '1px solid #E5E7EB', paddingBottom: '0.5rem' }}>
          Daily Medical Blog
        </h3>
        <BlogPosts />
      </div>
    </section>
  )
}
