# Template: API Endpoint

## Express.js Pattern

\`\`\`typescript
import { Router, Request, Response, NextFunction } from 'express';

const router = Router();

// Interface for request body
interface CreateResourceDTO {
  name: string;
  description?: string;
}

// Validation middleware
const validateResource = (req: Request, res: Response, next: NextFunction) => {
  if (!req.body.name) {
    return res.status(400).json({ error: 'Name is required' });
  }
  next();
};

// Create endpoint
router.post(
  '/resources',
  validateResource,
  async (req: Request, res: Response) => {
    try {
      const data: CreateResourceDTO = req.body;
      // Business logic here
      res.status(201).json({ success: true, data });
    } catch (error) {
      res.status(500).json({ error: error.message });
    }
  }
);

export default router;
\`\`\`

