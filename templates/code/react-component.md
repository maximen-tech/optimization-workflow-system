# Template: React Component

## Structure Standard

\`\`\`typescript
import React, { FC, ReactNode } from 'react';
import styles from './Component.module.css';

export interface ComponentProps {
  children: ReactNode;
  className?: string;
  // Add your props here
}

export const Component: FC<ComponentProps> = ({
  children,
  className = '',
}) => {
  // State & Hooks
  // Event Handlers
  // Effects
  
  return (
    <div className={\`\${styles.root} \${className}\`}>
      {children}
    </div>
  );
};

// Export with display name for debugging
Component.displayName = 'Component';

export default Component;
\`\`\`

## Tests Pattern

\`\`\`typescript
import { render, screen } from '@testing-library/react';
import { Component } from './Component';

describe('Component', () => {
  it('should render children', () => {
    render(<Component>Hello</Component>);
    expect(screen.getByText('Hello')).toBeInTheDocument();
  });
});
\`\`\`

